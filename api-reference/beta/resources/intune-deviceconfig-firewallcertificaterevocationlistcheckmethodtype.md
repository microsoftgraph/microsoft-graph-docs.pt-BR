---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3c1c9e4ae9068f6dc9d754da93a30979367e7587
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294498"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>tipo de enumeração firewallCertificateRevocationListCheckMethodType

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para firewallCertificateRevocationListCheckMethod

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário|
|nenhum|1|Não verificar a lista de certificados revogados|
|Houve|duas|Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação|
|precisa|3D|Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado|




