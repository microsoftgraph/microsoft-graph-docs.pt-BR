---
title: tipo de enum firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
ms.openlocfilehash: b6a7d702b1156598387c204d9e42b15f3066598d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006176"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>tipo de enum firewallCertificateRevocationListCheckMethodType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para firewallCertificateRevocationListCheckMethod
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário|
|nenhum|1|Não verificar a lista de revogação de certificado|
|tentativa|2|Tente verificação CRL e permitir que um certificado somente se o certificado for confirmado pela verificação de|
|exigir|3|Exigir uma verificação CRL bem-sucedida antes de permitir que um certificado|



