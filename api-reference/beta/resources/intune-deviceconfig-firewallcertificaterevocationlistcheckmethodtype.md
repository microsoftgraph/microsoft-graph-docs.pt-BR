---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74989961978ddd10f2c14e57cfe31e25ac831703
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170074"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>tipo de enumeração firewallCertificateRevocationListCheckMethodType

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para firewallCertificateRevocationListCheckMethod

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário|
|Nenhuma|1|Não verificar a lista de certificados revogados|
|Houve|duas|Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação|
|precisa|3D|Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado|




