---
title: tipo de enum firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2beee8f7c4f049aa1918b7e1516c3ce586a8cad0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839946"
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



