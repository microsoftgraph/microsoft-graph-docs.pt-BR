---
title: tipo denum groupPolicyConfigurationType
description: Tipo de configuração de política de grupo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 959e086703f0560e51dd8690f44d7dcce2da5ab6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805020"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a>tipo denum groupPolicyConfigurationType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de configuração de política de grupo

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|política|0|O tipo de política não faz a tatuagem do valor, o que significa que o valor é removido permitindo que o valor de configuração original seja usado. O tipo de política sobrecessa a configuração do aplicativo para que o aplicativo esteja sempre ciente do valor. O tipo de política impede que o usuário modifique o valor por meio da interface do usuário do aplicativo.|
|preference|1|O tipo de preferência faz a tatuagem do valor, o que significa que o valor não é removido do Registro. O tipo de preferência substituirá o valor configurado pelo usuário e não manterá o valor anterior. O tipo de preferência não impede que o usuário modifique o valor por meio da interface do usuário do aplicativo.|



