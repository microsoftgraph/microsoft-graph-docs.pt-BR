---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bdc653c07ad7553e9358703037c15179d9366dad
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722989"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="10567-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="10567-103">omaSetting resource type</span></span>

<span data-ttu-id="10567-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10567-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10567-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="10567-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10567-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10567-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10567-107">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="10567-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="10567-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10567-108">Properties</span></span>
|<span data-ttu-id="10567-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10567-109">Property</span></span>|<span data-ttu-id="10567-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="10567-110">Type</span></span>|<span data-ttu-id="10567-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="10567-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10567-112">displayName</span><span class="sxs-lookup"><span data-stu-id="10567-112">displayName</span></span>|<span data-ttu-id="10567-113">String</span><span class="sxs-lookup"><span data-stu-id="10567-113">String</span></span>|<span data-ttu-id="10567-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="10567-114">Display Name.</span></span>|
|<span data-ttu-id="10567-115">description</span><span class="sxs-lookup"><span data-stu-id="10567-115">description</span></span>|<span data-ttu-id="10567-116">String</span><span class="sxs-lookup"><span data-stu-id="10567-116">String</span></span>|<span data-ttu-id="10567-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="10567-117">Description.</span></span>|
|<span data-ttu-id="10567-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="10567-118">omaUri</span></span>|<span data-ttu-id="10567-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10567-119">String</span></span>|<span data-ttu-id="10567-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="10567-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10567-121">Relações</span><span class="sxs-lookup"><span data-stu-id="10567-121">Relationships</span></span>
<span data-ttu-id="10567-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10567-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10567-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10567-123">JSON Representation</span></span>
<span data-ttu-id="10567-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10567-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```





