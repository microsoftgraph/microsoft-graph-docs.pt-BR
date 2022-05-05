---
title: Tipo de enumeração zebraFotaNetworkType
description: Representa vários tipos de rede para a implantação do Zebra FOTA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9026673271e63ab386ad7a2c16a9fbc276ea52ba
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213052"
---
# <a name="zebrafotanetworktype-enum-type"></a>Tipo de enumeração zebraFotaNetworkType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa vários tipos de rede para a implantação do Zebra FOTA.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|qualquer|0|O dispositivo instalará a atualização independentemente do tipo de rede atual.|
|Wifi|1|O dispositivo instalará a atualização somente quando conectado à rede Wi-Fi.|
|Celular|2|O dispositivo instalará a atualização somente quando estiver conectado a uma rede celular.|
|wifiAndCellular|3|O dispositivo instalará a atualização quando conectado wi-fi e celular.|
|unknownFutureValue|99|Valor de enumeração futuro desconhecido.|




