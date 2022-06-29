---
title: Atualizações de software com o serviço Windows Update implantação do Windows Update Business
description: As atualizações de software são o tipo principal de conteúdo que o serviço de implantação implanta. Você pode procurar em um catálogo para encontrar atualizações específicas que estão disponíveis para implantação.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 206fe1fd09caacbf4db8715104fba54eefd9e113
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437391"
---
# <a name="software-updates-with-the-windows-update-for-business-deployment-service"></a>Atualizações de software com o serviço Windows Update implantação do Windows Update Business

As atualizações de software são o tipo principal de conteúdo que o serviço de implantação implanta. Você pode procurar em um catálogo para encontrar atualizações específicas que estão disponíveis para implantação.

Talvez você já esteja familiarizado com o [Catálogo do Microsoft Update](https://www.catalog.update.microsoft.com/), que lista as atualizações de software para Windows. O serviço de implantação fornece seu próprio [catálogo](/graph/api/resources/windowsupdates-catalog) e agrega atualizações equivalentes em um único [catalogEntry](/graph/api/resources/windowsupdates-catalogentry) para simplificar a tomada de decisão e os fluxos de trabalho de aprovação.

## <a name="windows-update-categories"></a>Categorias de atualização do Windows

Em geral, há duas categorias de alto nível de atualizações de Windows 10: atualizações de recursos e atualizações de qualidade. A queda na categoria de atualizações de qualidade inclui atualizações de segurança, atualizações de driver e outros.

O catálogo de serviços [de implantação](/graph/api/resources/windowsupdates-catalog?view=graph-rest-beta&preserve-view=true) também categoriza atualizações como atualizações de recursos e qualidade. [As entradas do catálogo de atualizações de](/graph/api/resources/windowsupdates-qualityupdatecatalogentry?view=graph-rest-beta&preserve-view=true) qualidade definem atualizações de segurança e não segurança de uma maneira específica e excluem atualizações de driver. Observe que a definição é diferente do Catálogo do Microsoft Update. Confira [as atualizações de qualidade](#quality-updates) abaixo para obter mais detalhes.

Efetivamente, o serviço de implantação atualmente implanta apenas atualizações de  recursos e atualizações de qualidade de segurança, conforme definido em seu catálogo. Atualmente, o serviço não implanta atualizações de qualidade de não segurança ou atualizações de driver.

Para saber mais sobre Windows 10 e manutenção, confira [o Guia Rápido para Windows como serviço](/windows/deployment/update/waas-quick-start).

## <a name="identifying-updates-for-deployment"></a>Identificando atualizações para implantação

As atualizações no Catálogo do Microsoft Update são muito granulares e específicas para produtos, versões e arquiteturas de CPU individuais. 

Por exemplo, as duas atualizações de qualidade de segurança a seguir são consideradas versões diferentes no Catálogo do Microsoft Update, mesmo que elas diferem apenas pela arquitetura.

| Título                                                                                   | Produtos                           | Classificação   |
|-----------------------------------------------------------------------------------------|------------------------------------|------------------|
| Atualização cumulativa 2021-03 para Windows 10 versão 20H2 para **sistemas baseados em x86** (KB5000802) | Windows 10, versão 1903 e posterior | Segurança Atualizações |
| Atualização cumulativa 2021-03 para Windows 10 versão 20H2 para **sistemas baseados em x64** (KB5000802) | Windows 10, versão 1903 e posterior | Segurança Atualizações |

No catálogo fornecido pelo serviço de implantação do Windows Update for Business, essas atualizações são agregadas em uma única entrada.

| Nome de exibição                                           | Tipo                                                     |
|--------------------------------------------------------|----------------------------------------------------------|
| 09/03/2021 – 2021.03 B Segurança Atualizações para Windows 10 | microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry |

Essa agregação simplifica o processo de aprovação de atualizações em uma base instalada diversificada. Da mesma forma, o serviço de implantação acumula versões de atualização de recursos.

### <a name="common-properties"></a>Propriedades comuns

Todas as atualizações no catálogo de serviços de implantação têm as propriedades comuns a seguir.

| Propriedade                | Descrição                                                        |
|-------------------------|--------------------------------------------------------------------|
| id                      | Identificador exclusivo para a entrada do catálogo.                           |
| displayName             | Título da atualização de software.                                      |
| releaseDateTime         | Data e hora em que a atualização foi lançada ou atualizada.                |
| deployableUntilDateTime | Data e hora até que a atualização não possa mais ser implantada, se conhecida.|

### <a name="feature-updates"></a>Atualizações de recursos

As atualizações de recursos no catálogo de serviços de implantação são identificadas por versão. As entradas agregam diferenças entre arquitetura (por exemplo, x86 vs. x64) e produto (no Catálogo do Microsoft Update, todas as atualizações de recursos são para o *Windows 10 produto).*

| Propriedade | Descrição                                       |
|----------|---------------------------------------------------|
| versão  | Versão de atualização de recursos para Windows 10 versão.|

Abaixo estão alguns exemplos de atualizações de recursos no catálogo de serviços de implantação.

| Nome de exibição                               | Versão |
|--------------------------------------------|---------|
| Atualização de recursos para Windows 10, versão 20H1 | 20H1    |
| Atualização de recursos para Windows 10, versão 1909 | 1909    |
| Atualização de recursos para Windows 10, versão 1903 | 1903    |
| Atualização de recursos para Windows 10, versão 1809 | 1809    |

Depois de identificar uma versão desejada, atribua-a como conteúdo a uma implantação usando [um featureUpdateReference](/graph/api/resources/windowsupdates-featureupdatereference) e especificando a propriedade **de** versão.

### <a name="quality-updates"></a>Atualizações de qualidade

As atualizações de qualidade no catálogo de serviços de implantação são identificadas por uma data/hora de lançamento e uma classificação de atualização. As entradas agregam diferenças entre arquitetura, produto (por exemplo *, Windows 10, versão 1903* e posterior versus *Windows 10* versus *Windows 10 LTSB*) e a versão de atualização de recursos correspondente.

| Propriedade | Descrição |
|----------|-------------|
| classificação | Classificação (segurança ou não segurança) da atualização de qualidade. |
| releaseDateTime | Data e hora em que a atualização foi lançada ou atualizada. |

A tabela a seguir mostra o mapeamento de classificação entre o catálogo de serviços de implantação e o Catálogo do Microsoft Update.

| Catálogo de serviços de implantação | Catálogo do Microsoft Update                                                                                                               |
|------------------|--------------------------------------------------------------------------------------------------------------------------------|
| Segurança         | Atualização de Segurança<br>Atualização crítica<br>Atualizar (se necessário como uma dependência)<br>Atualização da pilha de manutenção (se necessário como uma dependência) |
| Não segurança     | Atualizar<br>Atualização da pilha de manutenção                                                                                               |

As entradas do Catálogo do Microsoft Update correspondentes a `classification = security` `releaseDateTime = 2021-03-09` uma atualização de qualidade no catálogo de serviços de implantação com e podem incluir o seguinte.

| Título                                                                                   | Produtos                           | Classificação   |
|-----------------------------------------------------------------------------------------|------------------------------------|------------------|
| Atualização cumulativa 2021-03 para Windows 10 versão 20H2 para sistemas baseados em x86 (KB5000802) | Windows 10, versão 1903 e posterior | Segurança Atualizações |
| Atualização cumulativa 2021-03 para Windows 10 versão 20H2 para sistemas baseados em x64 (KB5000802) | Windows 10, versão 1903 e posterior | Segurança Atualizações |
| Atualização cumulativa 2021-03 para Windows 10 versão 1909 para sistemas baseados em x86 (KB5000808) | Windows 10, versão 1903 e posterior | Segurança Atualizações |
| Atualização cumulativa 2021-03 para Windows 10 versão 1809 para sistemas baseados em x64 (KB5000822) | Windows 10, Windows 10 LTSB        | Segurança Atualizações |

Depois de identificar a atualização desejada, atribua-a como conteúdo a uma implantação usando [um qualityUpdateReference](/graph/api/resources/windowsupdates-qualityupdatereference) e especificando as **propriedades releaseDateTime** **e classificação** .

## <a name="examples"></a>Exemplos

Para ver exemplos de [listagem de entradas de catálogo](/graph/api/windowsupdates-catalog-list-entries), consulte [Implantar uma atualização de recursos](windowsupdates-deploy-update.md) e [implantar uma atualização de segurança acelerada](windowsupdates-deploy-expedited-update.md).
