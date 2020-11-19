---
title: tipo de recurso customSubjectAlternativeName
description: Definição do nome alternativo da entidade personalizada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 461689c439d31a6c34a4e91ff758eba2c8d98b61
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256719"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="95548-103">tipo de recurso customSubjectAlternativeName</span><span class="sxs-lookup"><span data-stu-id="95548-103">customSubjectAlternativeName resource type</span></span>

<span data-ttu-id="95548-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95548-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95548-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="95548-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95548-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="95548-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95548-107">Definição do nome alternativo da entidade personalizada</span><span class="sxs-lookup"><span data-stu-id="95548-107">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="95548-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95548-108">Properties</span></span>
|<span data-ttu-id="95548-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95548-109">Property</span></span>|<span data-ttu-id="95548-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="95548-110">Type</span></span>|<span data-ttu-id="95548-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="95548-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95548-112">sanType</span><span class="sxs-lookup"><span data-stu-id="95548-112">sanType</span></span>|[<span data-ttu-id="95548-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="95548-113">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="95548-114">Tipo de SAN personalizado.</span><span class="sxs-lookup"><span data-stu-id="95548-114">Custom SAN Type.</span></span> <span data-ttu-id="95548-115">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="95548-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="95548-116">nome</span><span class="sxs-lookup"><span data-stu-id="95548-116">name</span></span>|<span data-ttu-id="95548-117">String</span><span class="sxs-lookup"><span data-stu-id="95548-117">String</span></span>|<span data-ttu-id="95548-118">Nome da SAN personalizada</span><span class="sxs-lookup"><span data-stu-id="95548-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="95548-119">Relações</span><span class="sxs-lookup"><span data-stu-id="95548-119">Relationships</span></span>
<span data-ttu-id="95548-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="95548-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95548-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95548-121">JSON Representation</span></span>
<span data-ttu-id="95548-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="95548-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```




