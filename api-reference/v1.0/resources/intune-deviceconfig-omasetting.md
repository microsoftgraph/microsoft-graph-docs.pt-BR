---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cffa929a063c77010f005a4e0b3da8fd8b7363d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530597"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="3772a-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="3772a-103">omaSetting resource type</span></span>

<span data-ttu-id="3772a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3772a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3772a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3772a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3772a-106">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="3772a-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="3772a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3772a-107">Properties</span></span>
|<span data-ttu-id="3772a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3772a-108">Property</span></span>|<span data-ttu-id="3772a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3772a-109">Type</span></span>|<span data-ttu-id="3772a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3772a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3772a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="3772a-111">displayName</span></span>|<span data-ttu-id="3772a-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3772a-112">String</span></span>|<span data-ttu-id="3772a-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="3772a-113">Display Name.</span></span>|
|<span data-ttu-id="3772a-114">description</span><span class="sxs-lookup"><span data-stu-id="3772a-114">description</span></span>|<span data-ttu-id="3772a-115">String</span><span class="sxs-lookup"><span data-stu-id="3772a-115">String</span></span>|<span data-ttu-id="3772a-116">Descrição.</span><span class="sxs-lookup"><span data-stu-id="3772a-116">Description.</span></span>|
|<span data-ttu-id="3772a-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="3772a-117">omaUri</span></span>|<span data-ttu-id="3772a-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3772a-118">String</span></span>|<span data-ttu-id="3772a-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="3772a-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3772a-120">Relações</span><span class="sxs-lookup"><span data-stu-id="3772a-120">Relationships</span></span>
<span data-ttu-id="3772a-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3772a-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3772a-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3772a-122">JSON Representation</span></span>
<span data-ttu-id="3772a-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3772a-123">Here is a JSON representation of the resource.</span></span>
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




