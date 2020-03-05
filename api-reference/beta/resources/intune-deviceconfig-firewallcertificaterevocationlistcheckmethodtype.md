---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4c9a94dc19064fc01d70bfa1123d20fec414eac0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526441"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>tipo de enumeração firewallCertificateRevocationListCheckMethodType

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para firewallCertificateRevocationListCheckMethod

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário|
|nenhuma|1 |Não verificar a lista de certificados revogados|
|Houve|2 |Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação|
|precisa|3 |Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado|



