---
title: tipo de número firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4cc592c2213cef70af497c9f3f4779bcae88e5694599a5d0f3fff50ac7d8b56e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189580"
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




