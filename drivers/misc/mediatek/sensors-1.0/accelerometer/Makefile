# In case the platform does NOT support this type of sensors
ccflags-y += -I$(srctree)/drivers/misc/mediatek/sensors-1.0/hwmon/include
ccflags-y += -I$(srctree)/drivers/misc/mediatek/sensors-1.0/include

obj-y   +=  accel.o accel_factory.o

obj-$(CONFIG_MTK_ACCELHUB)		+=	accelhub/
obj-$(CONFIG_MTK_MC3433)   +=  mc3433/
obj-$(CONFIG_MTK_LSM6DS3HG)   +=  lsm6ds3hg/
#add by yanghongjiang for add new driver
obj-$(CONFIG_MTK_BMI160_NEW)		+=	bmi160_acc/
#end
