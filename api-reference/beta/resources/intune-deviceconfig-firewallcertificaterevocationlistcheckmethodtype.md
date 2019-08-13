---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 832df7bfacbbba9643f4e1181f454bc60038ffb0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338151"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>tipo de enumeração firewallCertificateRevocationListCheckMethodType

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para firewallCertificateRevocationListCheckMethod

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário|
|none|1|Não verificar a lista de certificados revogados|
|Houve|duas|Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação|
|precisa|3D|Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado|



