---
title: Tipo de recurso deviceManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8c0d862f3b1a3658fb22dd4b320c0ca0dc597e04
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759440"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="00f26-103">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="00f26-103">deviceManagement resource type</span></span>

<span data-ttu-id="00f26-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00f26-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00f26-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="00f26-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00f26-106">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="00f26-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="00f26-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="00f26-107">Methods</span></span>
|<span data-ttu-id="00f26-108">Método</span><span class="sxs-lookup"><span data-stu-id="00f26-108">Method</span></span>|<span data-ttu-id="00f26-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="00f26-109">Return Type</span></span>|<span data-ttu-id="00f26-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="00f26-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="00f26-111">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="00f26-111">Get deviceManagement</span></span>](../api/intune-companyterms-devicemanagement-get.md)|[<span data-ttu-id="00f26-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="00f26-112">deviceManagement</span></span>](../resources/intune-companyterms-devicemanagement.md)|<span data-ttu-id="00f26-113">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-companyterms-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="00f26-113">Read properties and relationships of the [deviceManagement](../resources/intune-companyterms-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="00f26-114">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="00f26-114">Update deviceManagement</span></span>](../api/intune-companyterms-devicemanagement-update.md)|[<span data-ttu-id="00f26-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="00f26-115">deviceManagement</span></span>](../resources/intune-companyterms-devicemanagement.md)|<span data-ttu-id="00f26-116">Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune-companyterms-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="00f26-116">Update the properties of a [deviceManagement](../resources/intune-companyterms-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="00f26-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00f26-117">Properties</span></span>
|<span data-ttu-id="00f26-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00f26-118">Property</span></span>|<span data-ttu-id="00f26-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="00f26-119">Type</span></span>|<span data-ttu-id="00f26-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="00f26-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00f26-121">id</span><span class="sxs-lookup"><span data-stu-id="00f26-121">id</span></span>|<span data-ttu-id="00f26-122">String</span><span class="sxs-lookup"><span data-stu-id="00f26-122">String</span></span>|<span data-ttu-id="00f26-123">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="00f26-123">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="00f26-124">Relações</span><span class="sxs-lookup"><span data-stu-id="00f26-124">Relationships</span></span>
|<span data-ttu-id="00f26-125">Relação</span><span class="sxs-lookup"><span data-stu-id="00f26-125">Relationship</span></span>|<span data-ttu-id="00f26-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="00f26-126">Type</span></span>|<span data-ttu-id="00f26-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="00f26-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00f26-128">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="00f26-128">termsAndConditions</span></span>|<span data-ttu-id="00f26-129">Conjunto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)</span><span class="sxs-lookup"><span data-stu-id="00f26-129">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) collection</span></span>|<span data-ttu-id="00f26-130">Os termos e condições associados ao gerenciamento do dispositivo da empresa.</span><span class="sxs-lookup"><span data-stu-id="00f26-130">The terms and conditions associated with device management of the company.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00f26-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00f26-131">JSON Representation</span></span>
<span data-ttu-id="00f26-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00f26-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```




