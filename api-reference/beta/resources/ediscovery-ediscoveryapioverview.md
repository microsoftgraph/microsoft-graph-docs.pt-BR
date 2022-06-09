---
title: Use a API de Descoberta Eletrônica do Microsoft Graph
description: As APIs de descoberta eletrônica do Microsoft 365 fornecem funcionalidade para que as organizações automatizem tarefas repetitivas e se integrem às ferramentas de descoberta eletrônica existentes para criar fluxos de trabalho repetíveis que podem ser necessários com base nas regulamentações do setor. Você pode usar as APIs de descoberta eletrônica para ajudá-lo em suas necessidades legais.
ms.localizationpriority: high
author: mahage-msft
ms.prod: ediscovery
doc_type: conceptualPageType
ms.openlocfilehash: b5154880913e25ca6ed90a19695ff1c103a42eea
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944938"
---
# <a name="use-the-microsoft-graph-ediscovery-api"></a>Usar a API de Descoberta Eletrônica do Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As APIs do Microsoft Graph para Descoberta eletrônica fornecem funcionalidade para que as organizações automatizem tarefas repetitivas e se integrem com suas ferramentas de Descoberta eletrônica existentes para criar fluxos de trabalho repetíveis que podem ser necessários com base nas regulamentações do setor. Você pode usar as APIs de Descoberta eletrônica para ajudá-lo em suas necessidades legais.

> [!IMPORTANT]
> As APIs do Microsoft Graph para Descoberta Eletrônica destinam-se ao uso de operações de Descoberta Eletrônica para requisições de litígio, investigação e regulamentação. Essas APIs não devem ser usadas como um substituto para os dados de registro no diário do sistema Microsoft 365 ou qualquer outro download em massa.

> [!NOTE]
> Durante a visualização, o uso destas APIs pode exigir uma assinaturas de ofertas específicas da Microsoft e está sujeito aos [Termos de Uso de APIs Microsoft](/legal/microsoft-apis/terms-of-use?context=graph%252fcontext).  Mediante disponibilidade geral, a Microsoft pode exigir que você ou o seu cliente paguem taxas adicionais.
>
> Atualmente, as APIs de Descoberta Eletrônica no Microsoft Graph funcionam apenas em casos de Descoberta Eletrônica Avançada.

> [!CAUTION]
> As APIs de Descoberta Eletrônica no subnamespace de Descoberta Eletrônica estão sendo preteridas. Use as novas [APIs de Descoberta Eletrônica em segurança](security-api-overview.md#ediscovery-preview).

A API da Descoberta Eletrônica é definida no subnamespace OData, microsoft.graph.ediscovery. A API inclui as seguintes entidades principais.

| Nome | Tipo       | Caso de uso |
|:-|:-|:-|
| Caso | [microsoft.graph.ediscovery.case](ediscovery-case.md) | O contêiner para todos os objetos de Descoberta Eletrônica, incluindo custodiantes, retenções, pesquisas, conjuntos de revisões e exportações. |
| Custodian | [microsoft.graph.ediscovery.custodian](ediscovery-custodian.md) | Uma pessoa e os dados sobre os quais ela tem controle administrativo. Quando os custodiantes são identificados, *Descoberta Eletrônica Avançada* pode armazenar, pesquisar, selecionar e exportar seus dados. Para detalhes, consulte [Trabalhar com custodiantes e fontes de dados não custodiais na Descoberta Eletrônica Avançada](/microsoft-365/compliance/managing-custodians).|
| Retenção legal | [microsoft.graph.ediscovery.legalHold](ediscovery-legalhold.md) | Usado para retenção de conteúdo para litígios e propósitos legais. A retenção de informações legais não deve ser confundida ou usada como guarda de documentos, que normalmente é usada para cumprir regulamentações governamentais ou do setor. Para saber mais, consulte [Gerenciar retenções na Descoberta Eletrônica Avançada](/microsoft-365/compliance/managing-holds).|
| Conjuntos de revisão| [microsoft.graph.ediscovery.reviewSet](ediscovery-reviewset.md) | Um conjunto estático de informações armazenadas eletronicamente coletadas para uso em um litígio, investigação ou solicitação regulatória. |
| Resumo do conjunto de consulta | [microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) | Usado para descobrir, selecionar, revisar e marcar [ESI](https://en.wikipedia.org/wiki/Electronically_stored_information_(Federal_Rules_of_Civil_Procedure)) com o objetivo de produção para o solicitante ou advogado oposto.|
| Coleção fonte| [microsoft.graph.ediscovery.sourceCollection](ediscovery-sourcecollection.md)| Comumente conhecido como pesquisas, permite que você colete dados dos serviços ativos do Microsoft 365, como Exchange, SharePoint e Teams. Coleções de fontes podem ser adicionadas a um conjunto de revisões para selecionar e, eventualmente, exportar dados relevantes para o seu caso. Para detalhes, consulte [Coletar dados para um caso na Descoberta Eletrônica Avançada](/microsoft-365/compliance/collecting-data-for-ediscovery).|
| Marcas | [microsoft.graph.ediscovery.tag](ediscovery-tag.md) | Usado em um conjunto de revisão durante a revisão ou seleção para separar dados responsivos de dados não responsivos, identificar conteúdo privilegiado ou geralmente ajudar no processo de revisão.  Para mais, consulte [Identificar documentos em um conjunto de revisões em Descoberta Eletrônica Avançada](/microsoft-365/compliance/tagging-documents).|