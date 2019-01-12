---
title: tipo de enum firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 915fab77e7a2c28ab9d6902f3e1cb7d2d05cb2b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958408"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>tipo de enum firewallCertificateRevocationListCheckMethodType

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para firewallCertificateRevocationListCheckMethod
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário|
|nenhum|1|Não verificar a lista de revogação de certificado|
|tentativa|2|Tente verificação CRL e permitir que um certificado somente se o certificado for confirmado pela verificação de|
|exigir|3|Exigir uma verificação CRL bem-sucedida antes de permitir que um certificado|





