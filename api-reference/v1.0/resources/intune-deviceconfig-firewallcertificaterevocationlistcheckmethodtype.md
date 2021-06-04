---
title: tipo de número firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 779cfe8b8576d475df62ed112709aa0c2e9b6c63
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754724"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>tipo de número firewallCertificateRevocationListCheckMethodType

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para firewallCertificateRevocationListCheckMethod

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário|
|nenhuma|1|Não verificar lista de revogação de certificado|
|tentativa|2|Tente verificar CRL e permitir um certificado somente se o certificado for confirmado pela verificação|
|require|3|Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado|




