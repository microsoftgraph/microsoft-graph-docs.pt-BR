---
title: tipo denum groupPolicyConfigurationType
description: Tipo de configuração de política de grupo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9c840543269d8c3f81a63c8717eaf598bf2ad94049c856cee3a16f3503111d98
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54253534"
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
|preference|1 |O tipo de preferência faz a tatuagem do valor, o que significa que o valor não é removido do Registro. O tipo de preferência substituirá o valor configurado pelo usuário e não manterá o valor anterior. O tipo de preferência não impede que o usuário modifique o valor por meio da interface do usuário do aplicativo.|




