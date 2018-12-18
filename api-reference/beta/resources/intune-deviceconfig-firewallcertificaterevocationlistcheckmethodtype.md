---
title: tipo de enum firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: tfitzmac
ms.openlocfilehash: 302037187addfb8606c6c1e60a9369eb1f7c2ed5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320710"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>tipo de enum firewallCertificateRevocationListCheckMethodType

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para firewallCertificateRevocationListCheckMethod
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário|
|none|1|Não verificar a lista de revogação de certificado|
|tentativa|2|Tente verificação CRL e permitir que um certificado somente se o certificado for confirmado pela verificação de|
|exigir|3|Exigir uma verificação CRL bem-sucedida antes de permitir que um certificado|





