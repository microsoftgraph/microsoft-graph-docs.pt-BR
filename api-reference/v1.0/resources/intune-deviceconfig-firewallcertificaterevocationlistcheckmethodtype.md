---
title: tipo de número firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9bc65e8f210d3d2a7cba2754e2d73ea2a448206e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139832"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>tipo de número firewallCertificateRevocationListCheckMethodType

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para firewallCertificateRevocationListCheckMethod

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário|
|Nenhuma|1|Não verificar lista de revogação de certificado|
|tentativa|2|Tente verificar CRL e permitir um certificado somente se o certificado for confirmado pela verificação|
|require|3|Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado|




