---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 59a0d38eca6e448457d208eb9981c9de51031489
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273183"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="3c755-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="3c755-103">omaSetting resource type</span></span>

<span data-ttu-id="3c755-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c755-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c755-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c755-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c755-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c755-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c755-107">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="3c755-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="3c755-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c755-108">Properties</span></span>
|<span data-ttu-id="3c755-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c755-109">Property</span></span>|<span data-ttu-id="3c755-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c755-110">Type</span></span>|<span data-ttu-id="3c755-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c755-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c755-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3c755-112">displayName</span></span>|<span data-ttu-id="3c755-113">String</span><span class="sxs-lookup"><span data-stu-id="3c755-113">String</span></span>|<span data-ttu-id="3c755-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="3c755-114">Display Name.</span></span>|
|<span data-ttu-id="3c755-115">description</span><span class="sxs-lookup"><span data-stu-id="3c755-115">description</span></span>|<span data-ttu-id="3c755-116">String</span><span class="sxs-lookup"><span data-stu-id="3c755-116">String</span></span>|<span data-ttu-id="3c755-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="3c755-117">Description.</span></span>|
|<span data-ttu-id="3c755-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="3c755-118">omaUri</span></span>|<span data-ttu-id="3c755-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c755-119">String</span></span>|<span data-ttu-id="3c755-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="3c755-120">OMA.</span></span>|
|<span data-ttu-id="3c755-121">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="3c755-121">isEncrypted</span></span>|<span data-ttu-id="3c755-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c755-122">Boolean</span></span>|<span data-ttu-id="3c755-123">Indica se o campo de valor é criptografado.</span><span class="sxs-lookup"><span data-stu-id="3c755-123">Indicates whether the value field is encrypted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c755-124">Relações</span><span class="sxs-lookup"><span data-stu-id="3c755-124">Relationships</span></span>
<span data-ttu-id="3c755-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c755-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c755-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c755-126">JSON Representation</span></span>
<span data-ttu-id="3c755-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c755-127">Here is a JSON representation of the resource.</span></span>
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
  "omaUri": "String",
  "isEncrypted": true
}
```




