---
title: Atualizações de software com o serviço de implantação Windows Update for Business
description: As atualizações de software são o tipo principal de conteúdo implantado pelo serviço de implantação. Você pode procurar em um catálogo para encontrar atualizações específicas disponíveis para implantar.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 3f3dd0a1da1c6426c8415fe3c6f37767d1613627
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072233"
---
# <a name="software-updates-with-the-windows-update-for-business-deployment-service"></a>Atualizações de software com o serviço de implantação Windows Update for Business

As atualizações de software são o tipo principal de conteúdo implantado pelo serviço de implantação. Você pode procurar em um catálogo para encontrar atualizações específicas disponíveis para implantar.

Você pode já estar familiarizado com o [Catálogo de Atualizações](https://www.catalog.update.microsoft.com/) da Microsoft que lista atualizações de software para Windows. O serviço de implantação fornece seu próprio [catálogo](/graph/api/resources/windowsupdates-catalog)e agrega atualizações equivalentes em um único [catalogEntry](/graph/api/resources/windowsupdates-catalogentry) para simplificar a tomada de decisões e os fluxos de trabalho de aprovação.

## <a name="windows-update-categories"></a>Categorias de atualização do Windows

Em geral, há duas categorias de alto nível de Windows 10 atualizações: atualizações de recursos e atualizações de qualidade. A categoria atualizações de qualidade inclui atualizações de segurança, atualizações de driver e outras.

O catálogo de serviços [de implantação](/graph/api/resources/windowsupdates-catalog?view=graph-rest-beta&preserve-view=true) também categoriza atualizações como atualizações de recursos e qualidade. [As entradas do catálogo de atualizações de](/graph/api/resources/windowsupdates-qualityupdatecatalogentry?view=graph-rest-beta&preserve-view=true) qualidade definem atualizações de segurança e não de segurança de uma maneira específica e excluam atualizações de driver. Observe que a definição é diferente do Catálogo de Atualizações da Microsoft. Confira [atualizações de qualidade](#quality-updates) abaixo para obter mais detalhes.

Efetivamente, o serviço de implantação atualmente  implanta apenas atualizações de recursos e atualizações de qualidade de segurança, conforme definido em seu catálogo. No momento, o serviço não implanta atualizações de qualidade não segurança ou atualizações de driver.

Para saber mais sobre Windows 10 atualizações e manutenção, consulte [Guia rápido para Windows como serviço](/windows/deployment/update/waas-quick-start).

## <a name="identifying-updates-for-deployment"></a>Identificar atualizações para implantação

As atualizações no Catálogo de Atualizações da Microsoft são muito granulares e específicas para produtos individuais, versões e arquiteturas de CPU. 

Por exemplo, as duas atualizações de qualidade de segurança a seguir são consideradas versões diferentes no Catálogo de Atualizações da Microsoft, embora sejam diferentes apenas pela arquitetura.

| Título                                                                                   | Produtos                           | Classificação   |
|-----------------------------------------------------------------------------------------|------------------------------------|------------------|
| Atualização Cumulativa 2021-03 para Windows 10 versão 20H2 para sistemas baseados em **x86**(KB5000802) | Windows 10, versão 1903 e posterior | Atualizações de segurança |
| Atualização Cumulativa 2021-03 para Windows 10 versão 20H2 para sistemas baseados em **x64**(KB5000802) | Windows 10, versão 1903 e posterior | Atualizações de segurança |

No catálogo fornecido pelo serviço de implantação Windows Update for Business, essas atualizações são agregadas em uma única entrada.

| Nome de exibição                                           | Tipo                                                     |
|--------------------------------------------------------|----------------------------------------------------------|
| 03/09/2021 - Atualizações de segurança de 2021.03 B para Windows 10 | microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry |

Essa agregação simplifica o processo de aprovação de atualizações em uma base instalada diversificada. Da mesma forma, o serviço de implantação implementa versões de atualização de recursos.

### <a name="common-properties"></a>Propriedades comuns

Todas as atualizações no catálogo de serviços de implantação têm as seguintes propriedades comuns.

| Propriedade                | Descrição                                                        |
|-------------------------|--------------------------------------------------------------------|
| id                      | Identificador exclusivo para a entrada do catálogo.                           |
| displayName             | Título da atualização de software.                                      |
| releaseDateTime         | Data e hora em que a atualização foi lançada ou atualizada.                |
| deployableUntilDateTime | Data e hora até que a atualização não possa mais ser implantada, se conhecida.|

### <a name="feature-updates"></a>Atualizações de recursos

As atualizações de recursos no catálogo de serviços de implantação são identificadas pela versão. Entradas agregam diferenças entre arquitetura (por exemplo, x86 vs. x64) e produto (no Catálogo de Atualizações da Microsoft, todas as atualizações de recursos são para o *produto Windows 10).*

| Propriedade | Descrição                                       |
|----------|---------------------------------------------------|
| versão  | Versão de atualização de recursos para o Windows 10 versão.|

Veja a seguir alguns exemplos de atualizações de recursos no catálogo de serviços de implantação.

| Nome                               | Versão |
|--------------------------------------------|---------|
| Atualização de recursos Windows 10 versão 20H1 | 20H1    |
| Atualização de recursos Windows 10 versão 1909 | 1909    |
| Atualização de recursos Windows 10 versão 1903 | 1903    |
| Atualização de recursos para Windows 10, versão 1809 | 1809    |

Depois de identificar uma versão desejada, atribua-a como conteúdo a uma implantação usando [um featureUpdateReference](/graph/api/resources/windowsupdates-featureupdatereference) e especificando a **propriedade version.**

### <a name="quality-updates"></a>Atualizações de qualidade

As atualizações de qualidade no catálogo de serviços de implantação são identificadas por uma data/hora de lançamento e uma classificação de atualização. As entradas *agregam* diferenças entre arquitetura, produto *(por exemplo, Windows 10, versão 1903* e posterior versus Windows 10 vs. *Windows 10 LTSB*) e a versão de atualização de recursos correspondente.

| Propriedade | Descrição |
|----------|-------------|
| classificação | Classificação (segurança ou não segurança) da atualização de qualidade. |
| releaseDateTime | Data e hora em que a atualização foi lançada ou atualizada. |

A tabela a seguir mostra o mapeamento de classificação entre o catálogo de serviços de implantação e o Catálogo de Atualizações da Microsoft.

| Catálogo de serviços de implantação | Catálogo do Microsoft Update                                                                                                               |
|------------------|--------------------------------------------------------------------------------------------------------------------------------|
| Segurança         | Atualização de Segurança<br>Atualização Crítica<br>Atualizar (se necessário como dependência)<br>Manutenção da Atualização de Pilha (se necessário como dependência) |
| Não segurança     | Atualizar<br>Atualização de Pilha de Manutenção                                                                                               |

As entradas do Catálogo de Atualizações da Microsoft correspondentes a uma atualização de qualidade no catálogo de serviços de implantação com e `classification = security` `releaseDateTime = 2021-03-09` podem incluir o seguinte.

| Título                                                                                   | Produtos                           | Classificação   |
|-----------------------------------------------------------------------------------------|------------------------------------|------------------|
| Atualização Cumulativa 2021-03 para Windows 10 versão 20H2 para sistemas baseados em x86 (KB5000802) | Windows 10, versão 1903 e posterior | Atualizações de segurança |
| Atualização Cumulativa 2021-03 para Windows 10 versão 20H2 para sistemas baseados em x64 (KB5000802) | Windows 10, versão 1903 e posterior | Atualizações de segurança |
| Atualização Cumulativa 2021-03 para Windows 10 versão 1909 para sistemas baseados em x86 (KB5000808) | Windows 10, versão 1903 e posterior | Atualizações de segurança |
| Atualização Cumulativa 2021-03 para Windows 10 versão 1809 para sistemas baseados em x64 (KB5000822) | Windows 10, Windows 10 LTSB        | Atualizações de segurança |

Depois de identificar a atualização desejada, atribua-a como conteúdo a uma implantação usando [uma qualityUpdateReference](/graph/api/resources/windowsupdates-qualityupdatereference) e especificando as **propriedades releaseDateTime** **e classificação.**

## <a name="examples"></a>Exemplos

Para ver exemplos de [entradas de catálogo de](/graph/api/windowsupdates-catalog-list-entries)listagem, consulte Deploy a feature [update](windowsupdates-deploy-update.md) and Deploy [an expedited security update](windowsupdates-deploy-expedited-update.md).