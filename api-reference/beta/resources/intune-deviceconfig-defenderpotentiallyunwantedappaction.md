---
title: tipo de enumeração defenderPotentiallyUnwantedAppAction
description: Ação do defender a ser executada em aplicativo potencialmente indesejado (PUA).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: aad2c9e37dfe3a3069caad25c7917a864c65a194
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256509"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>tipo de enumeração defenderPotentiallyUnwantedAppAction

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ação do defender a ser executada em aplicativo potencialmente indesejado (PUA).

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|A proteção do PUA está desativada. O defender não protegerá contra aplicativos potencialmente indesejados.|
|Larga|1|A proteção do PUA está ativada. Os itens detectados são bloqueados. Eles serão mostrados em histórico junto com outras ameaças.|
|Faça|duas|Modo de auditoria. O defender detectará aplicativos potencialmente indesejados, mas não realizará ações. Você pode revisar as informações sobre os aplicativos que o defender teria feito com a pesquisa de eventos criados pelo defender no Visualizador de eventos.|




