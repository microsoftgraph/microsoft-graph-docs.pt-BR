---
title: tipo de número firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1942fbbe5088e73d648740d7d8a7cb2c86aa7da8
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60446635"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>tipo de número firewallCertificateRevocationListCheckMethodType

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para firewallCertificateRevocationListCheckMethod

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário|
|none|1|Não verificar lista de revogação de certificado|
|tentativa|2|Tente verificar CRL e permitir um certificado somente se o certificado for confirmado pela verificação|
|require|3|Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado|



