---
title: tipo de recurso de mobileContainedApp
description: Uma classe abstrata que representa um aplicativo contido em um mobileApp atuando como um pacote.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c5d4ed392d681d97478cb1baf5ff6f854cb74011
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425663"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="da8a7-103">tipo de recurso de mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="da8a7-103">mobileContainedApp resource type</span></span>

> <span data-ttu-id="da8a7-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="da8a7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="da8a7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="da8a7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da8a7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="da8a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da8a7-107">Uma classe abstrata que representa um aplicativo contido em um mobileApp atuando como um pacote.</span><span class="sxs-lookup"><span data-stu-id="da8a7-107">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>

## <a name="methods"></a><span data-ttu-id="da8a7-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="da8a7-108">Methods</span></span>
|<span data-ttu-id="da8a7-109">Método</span><span class="sxs-lookup"><span data-stu-id="da8a7-109">Method</span></span>|<span data-ttu-id="da8a7-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="da8a7-110">Return Type</span></span>|<span data-ttu-id="da8a7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="da8a7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="da8a7-112">Lista mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="da8a7-112">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="da8a7-113">coleção [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="da8a7-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="da8a7-114">Lista as propriedades e os relacionamentos dos objetos [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="da8a7-114">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="da8a7-115">Obter mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="da8a7-115">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="da8a7-116">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="da8a7-116">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="da8a7-117">Leia as propriedades e os relacionamentos do objeto [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="da8a7-117">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="da8a7-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da8a7-118">Properties</span></span>
|<span data-ttu-id="da8a7-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da8a7-119">Property</span></span>|<span data-ttu-id="da8a7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="da8a7-120">Type</span></span>|<span data-ttu-id="da8a7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="da8a7-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da8a7-122">id</span><span class="sxs-lookup"><span data-stu-id="da8a7-122">id</span></span>|<span data-ttu-id="da8a7-123">String</span><span class="sxs-lookup"><span data-stu-id="da8a7-123">String</span></span>|<span data-ttu-id="da8a7-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="da8a7-124">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da8a7-125">Relações</span><span class="sxs-lookup"><span data-stu-id="da8a7-125">Relationships</span></span>
<span data-ttu-id="da8a7-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="da8a7-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da8a7-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da8a7-127">JSON Representation</span></span>
<span data-ttu-id="da8a7-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da8a7-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileContainedApp",
  "id": "String (identifier)"
}
```




