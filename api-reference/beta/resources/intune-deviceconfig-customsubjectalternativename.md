---
title: tipo de recurso customSubjectAlternativeName
description: Definição do nome alternativo da entidade personalizada
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b1583a88a52a626803fe45837e056ec020b05e2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146211"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="da672-103">tipo de recurso customSubjectAlternativeName</span><span class="sxs-lookup"><span data-stu-id="da672-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="da672-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="da672-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da672-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="da672-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da672-106">Definição do nome alternativo da entidade personalizada</span><span class="sxs-lookup"><span data-stu-id="da672-106">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="da672-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da672-107">Properties</span></span>
|<span data-ttu-id="da672-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da672-108">Property</span></span>|<span data-ttu-id="da672-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="da672-109">Type</span></span>|<span data-ttu-id="da672-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="da672-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da672-111">sanType</span><span class="sxs-lookup"><span data-stu-id="da672-111">sanType</span></span>|[<span data-ttu-id="da672-112">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="da672-112">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="da672-113">Tipo de SAN personalizado.</span><span class="sxs-lookup"><span data-stu-id="da672-113">Custom SAN Type.</span></span> <span data-ttu-id="da672-114">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="da672-114">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="da672-115">name</span><span class="sxs-lookup"><span data-stu-id="da672-115">name</span></span>|<span data-ttu-id="da672-116">String</span><span class="sxs-lookup"><span data-stu-id="da672-116">String</span></span>|<span data-ttu-id="da672-117">Nome da SAN personalizada</span><span class="sxs-lookup"><span data-stu-id="da672-117">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="da672-118">Relações</span><span class="sxs-lookup"><span data-stu-id="da672-118">Relationships</span></span>
<span data-ttu-id="da672-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="da672-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da672-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da672-120">JSON Representation</span></span>
<span data-ttu-id="da672-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da672-121">Here is a JSON representation of the resource.</span></span>
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




