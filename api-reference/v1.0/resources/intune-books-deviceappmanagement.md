---
title: Tipo de recurso deviceAppManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 972590f5666f140e75074dd674433716961a17e7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752830"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="6309e-103">Tipo de recurso deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="6309e-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="6309e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6309e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6309e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6309e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6309e-106">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6309e-106">Singleton entity that acts as a container for all device app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="6309e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6309e-107">Methods</span></span>
|<span data-ttu-id="6309e-108">Método</span><span class="sxs-lookup"><span data-stu-id="6309e-108">Method</span></span>|<span data-ttu-id="6309e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6309e-109">Return Type</span></span>|<span data-ttu-id="6309e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6309e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6309e-111">Obter deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="6309e-111">Get deviceAppManagement</span></span>](../api/intune-books-deviceappmanagement-get.md)|[<span data-ttu-id="6309e-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="6309e-112">deviceAppManagement</span></span>](../resources/intune-books-deviceappmanagement.md)|<span data-ttu-id="6309e-113">Ler propriedades e relações de objetos de [deviceAppManagement](../resources/intune-books-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="6309e-113">Read properties and relationships of the [deviceAppManagement](../resources/intune-books-deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="6309e-114">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="6309e-114">Update deviceAppManagement</span></span>](../api/intune-books-deviceappmanagement-update.md)|[<span data-ttu-id="6309e-115">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="6309e-115">deviceAppManagement</span></span>](../resources/intune-books-deviceappmanagement.md)|<span data-ttu-id="6309e-116">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-books-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="6309e-116">Update the properties of a [deviceAppManagement](../resources/intune-books-deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6309e-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6309e-117">Properties</span></span>
|<span data-ttu-id="6309e-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6309e-118">Property</span></span>|<span data-ttu-id="6309e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="6309e-119">Type</span></span>|<span data-ttu-id="6309e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6309e-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6309e-121">id</span><span class="sxs-lookup"><span data-stu-id="6309e-121">id</span></span>|<span data-ttu-id="6309e-122">String</span><span class="sxs-lookup"><span data-stu-id="6309e-122">String</span></span>|<span data-ttu-id="6309e-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6309e-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6309e-124">Relações</span><span class="sxs-lookup"><span data-stu-id="6309e-124">Relationships</span></span>
|<span data-ttu-id="6309e-125">Relação</span><span class="sxs-lookup"><span data-stu-id="6309e-125">Relationship</span></span>|<span data-ttu-id="6309e-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="6309e-126">Type</span></span>|<span data-ttu-id="6309e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="6309e-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6309e-128">managedEBooks</span><span class="sxs-lookup"><span data-stu-id="6309e-128">managedEBooks</span></span>|<span data-ttu-id="6309e-129">Conjunto [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="6309e-129">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="6309e-130">Livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="6309e-130">The Managed eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6309e-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6309e-131">JSON Representation</span></span>
<span data-ttu-id="6309e-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6309e-132">Here is a JSON representation of the resource.</span></span>
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




