#
# Makefile for Bosch sensor driver.
#

obj-$(CONFIG_BOSCH_DRIVER_LOG_FUNC) += bs_log.o
ifeq ($(CONFIG_BOSCH_DRIVER_LOG_FUNC),y)
	EXTRA_CFLAGS += -DBOSCH_DRIVER_LOG_FUNC
endif


obj-$(CONFIG_SENSORS_BMA2X2)    += bma2x2.o

ifeq ($(CONFIG_SENSORS_BMA2X2_ENABLE_INT1),y)
	EXTRA_CFLAGS += -DBMA2X2_ENABLE_INT1
endif

ifeq ($(CONFIG_BOSCH_BMA2X2_ENABLE_INT2),y)
	EXTRA_CFLAGS += -DBMA2X2_ENABLE_INT2
endif

obj-$(CONFIG_SENSORS_BMG)    += bmg160_driver.o bmg160.o
EXTRA_CFLAGS += -DBMG_USE_BASIC_I2C_FUNC


obj-$(CONFIG_SENSORS_BMM050)    += bmm050_driver.o bmm050.o
EXTRA_CFLAGS += -DBMM_USE_BASIC_I2C_FUNC -DCONFIG_BMM_USE_PLATFORM_DATA




