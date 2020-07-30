---
title: Use a API de Descoberta Eletrônica do Microsoft Graph
description: As APIs de Descoberta Eletrônica do Microsoft 365 fornecem funcionalidade para as organizações automatizarem as tarefas repetitivas e se integrarem às ferramentas existentes de Descoberta Eletrônica para criar um fluxo de trabalho repetível que pode ser necessário com base nos regulamentos do setor. Você pode usar as APIs de Descoberta Eletrônica para ajudar com as suas necessidades legais.
localization_priority: Priority
author: mahage-msft
ms.prod: compliance
doc_type: conceptualPageType
ms.openlocfilehash: 04cacac77e88dc5e7c266c39d5a48ffdd9d65cef
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509965"
---
# <a name="use-the-microsoft-graph-ediscovery-api"></a>Use a API de Descoberta Eletrônica do Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As APIs do Microsoft Graph para Descoberta Eletrônica fornecem funcionalidade para que as organizações automatizem as tarefas repetitivas e se integrem às suas ferramentas existentes de Descoberta Eletrônica para criar fluxos de trabalho repetíveis que podem ser necessários com base nos regulamentos do setor. Você pode usar as APIs de Descoberta Eletrônica para ajudar com as suas necessidades legais.

> [!IMPORTANT]
> As APIs do Microsoft Graph para Descoberta Eletrônica destinam-se ao uso de operações de Descoberta Eletrônica para requisições de Litígio, Investigação e regulamentação. Essas APIs não devem ser usadas como um substituto para os dados de registro no diário do sistema Microsoft 365 ou qualquer outro download em massa.

> [!NOTE]
> Durante a visualização, o uso destas APIs pode exigir uma assinaturas de ofertas específicas da Microsoft e está sujeito aos [Termos de Uso de APIs Microsoft](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).  Mediante disponibilidade geral, a Microsoft pode exigir que você ou o seu cliente paguem taxas adicionais.
>
> Atualmente, as APIs de Descoberta Eletrônica no Microsoft Graph funcionam apenas em casos de Descoberta Eletrônica Avançada.

A API do Microsoft Graph inclui as seguintes entidades principais.

| Nome | Tipo       | Caso de uso |
|:-|:-|:-|
| Caso de Descoberta Eletrônica | [ediscoveryCase](ediscoverycase.md) | Os casos de Descoberta Eletrônica são o contêiner para todos os objetos de Descoberta Eletrônica, incluindo custodiantes, retenções, pesquisas, conjunto de revisões e exportações. |
| Conjunto de revisão de Descoberta Eletrônica| [reviewSet](reviewset.md) | Os conjuntos de revisões de Descoberta Eletrônica são um conjunto estático de informações armazenadas eletronicamente coletadas para uso em um litígio, investigação ou solicitação regulatória. |
| Consulta do conjunto de revisão de Descoberta Eletrônica | [reviewSetQuery](reviewsetquery.md) | As consultas do conjunto de revisão de Descoberta Eletrônica são usadas para descobrir, selecionar, revisar e marcar [ ESI ](https://en.wikipedia.org/wiki/Electronically_stored_information_(Federal_Rules_of_Civil_Procedure)) com o objetivo final de produção para o solicitante ou o advogado adversário.

