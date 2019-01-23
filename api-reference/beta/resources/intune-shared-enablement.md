---
title: tipo de enum habilitação
description: Descreve a enumeração de habilitação da API Microsoft Graph para Intune, que oferece suporte a vários fluxos de trabalho.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 538b52790cf7748453adfda2a6bea8334a36fb87
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399560"
---
# <a name="enablement-enum-type"></a>tipo de enum habilitação

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores usados para indicar o status de um dispositivo. 

Observe que há uma diferença entre desabilitado e não configurado.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|não-configuradas|0|Valor de padrão de dispositivo, sem intenção.|
|enabled|1|Permite a configuração no dispositivo.|
|desabilitado|2|Desativa a configuração no dispositivo.|
