# To successfully include this file in your cmake structure, consider the following:
# Optional Variables:
#   STM32H5xx_HAL_DOXYGEN_OUTPUT_DIRECTORY Could be used for overriding the default doxygen output directory of STM32H5xx HAL
# Required Variables:
#   STM32H5xx_HAL_CONF HAL Configuration file of the MCU
 
get_filename_component(STM32H5xx_HAL_BASE_PATH "${CMAKE_CURRENT_LIST_DIR}" ABSOLUTE)
 
set(STM32H5_HAL_SOURCES
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_adc.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_adc_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_cec.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_comp.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_cordic.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_cortex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_crc.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_crc_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_cryp.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_cryp_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_dac.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_dac_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_dcache.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_dcmi.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_dma.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_dma_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_dts.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_eth.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_eth_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_exti.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_fdcan.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_flash.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_flash_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_fmac.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_gpio.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_gtzc.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_hash.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_hcd.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_i2c.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_i2c_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_i2s.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_i2s_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_i3c.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_icache.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_irda.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_iwdg.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_lptim.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_mmc.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_mmc_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_nand.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_nor.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_opamp.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_opamp_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_otfdec.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_pcd.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_pcd_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_pka.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_pssi.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_pwr.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_pwr_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_ramcfg.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_rcc.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_rcc_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_rng.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_rng_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_rtc.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_rtc_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_sai.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_sai_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_sd.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_sd_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_sdio.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_sdram.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_smartcard.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_smartcard_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_smbus.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_smbus_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_spi.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_spi_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_sram.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_tim.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_tim_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_uart.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_uart_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_usart.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_usart_ex.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_wwdg.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_hal_xspi.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_adc.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_comp.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_cordic.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_crc.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_crs.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_dac.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_dlyb.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_dma.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_exti.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_fmac.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_fmc.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_gpio.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_i2c.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_i3c.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_icache.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_lptim.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_lpuart.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_opamp.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_pka.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_pwr.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_rcc.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_rng.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_rtc.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_sdmmc.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_spi.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_tim.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_ucpd.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_usart.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_usb.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_ll_utils.c
${STM32H5xx_HAL_BASE_PATH}/Src/stm32h5xx_util_i3c.c
)
 
if(NOT TARGET Stm32h5xxHalConf)
  message(FATAL_ERROR "Target Stm32h5xxHalConf does not exist")
endif()
 
if(CMAKE_SYSTEM_PROCESSOR STREQUAL "arm")
 
  add_library(stm32h5xx-hal
    ${STM32H5_HAL_SOURCES}
    ${STM32H5_HAL_PATCH_SOURCES}
  )
 
  # The include directories are explicitly marked as non system includes as cmake apparently removes system include paths from the dependency tree
  target_include_directories(stm32h5xx-hal
    PUBLIC
      ${STM32H5xx_HAL_BASE_PATH}/patch/include
      ${STM32H5xx_HAL_BASE_PATH}/Inc
    )
 
  target_link_libraries(stm32h5xx-hal
    PUBLIC
      stm32h5-cmsis
      Stm32h5xxHalConf
    )
 
else()
 
  add_library(stm32h5xx-hal INTERFACE
    )
 
  # The include directories are explicitly marked as non system includes as cmake apparently removes system include paths from the dependency tree
  target_include_directories(stm32h5xx-hal
    INTERFACE
      ${STM32H5xx_HAL_BASE_PATH}/patch/include
      ${STM32H5xx_HAL_BASE_PATH}/Inc
    )
 
  target_link_libraries(stm32h5xx-hal
    INTERFACE
      stm32h5-cmsis
      Stm32h5xxHalConf
    )
 
endif()
 
# add_subdirectory(mock EXCLUDE_FROM_ALL)