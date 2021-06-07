---
title: Tipo de recurso deviceAppManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos e aplicativos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 783ba507373c90cee6ba3e646d085f1a6502c5cf
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751752"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="88014-103">Tipo de recurso deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="88014-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="88014-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88014-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88014-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88014-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88014-106">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="88014-106">Singleton entity that acts as a container for all device and app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="88014-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="88014-107">Methods</span></span>
|<span data-ttu-id="88014-108">Método</span><span class="sxs-lookup"><span data-stu-id="88014-108">Method</span></span>|<span data-ttu-id="88014-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="88014-109">Return Type</span></span>|<span data-ttu-id="88014-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="88014-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="88014-111">Obter deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="88014-111">Get deviceAppManagement</span></span>](../api/intune-policyset-deviceappmanagement-get.md)|[<span data-ttu-id="88014-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="88014-112">deviceAppManagement</span></span>](../resources/intune-policyset-deviceappmanagement.md)|<span data-ttu-id="88014-113">Ler propriedades e relações de objetos de [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="88014-113">Read properties and relationships of the [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="88014-114">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="88014-114">Update deviceAppManagement</span></span>](../api/intune-policyset-deviceappmanagement-update.md)|[<span data-ttu-id="88014-115">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="88014-115">deviceAppManagement</span></span>](../resources/intune-policyset-deviceappmanagement.md)|<span data-ttu-id="88014-116">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="88014-116">Update the properties of a [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="88014-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88014-117">Properties</span></span>
|<span data-ttu-id="88014-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88014-118">Property</span></span>|<span data-ttu-id="88014-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="88014-119">Type</span></span>|<span data-ttu-id="88014-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="88014-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88014-121">id</span><span class="sxs-lookup"><span data-stu-id="88014-121">id</span></span>|<span data-ttu-id="88014-122">String</span><span class="sxs-lookup"><span data-stu-id="88014-122">String</span></span>|<span data-ttu-id="88014-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="88014-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88014-124">Relações</span><span class="sxs-lookup"><span data-stu-id="88014-124">Relationships</span></span>
<span data-ttu-id="88014-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="88014-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88014-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88014-126">JSON Representation</span></span>
<span data-ttu-id="88014-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88014-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```




