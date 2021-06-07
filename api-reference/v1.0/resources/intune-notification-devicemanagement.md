---
title: Tipo de recurso deviceManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6e933d26aeea4b8225d590873bbfe270150aca8b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751791"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="8ab8c-103">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="8ab8c-103">deviceManagement resource type</span></span>

<span data-ttu-id="8ab8c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ab8c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ab8c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ab8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ab8c-106">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8ab8c-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="8ab8c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8ab8c-107">Methods</span></span>
|<span data-ttu-id="8ab8c-108">Método</span><span class="sxs-lookup"><span data-stu-id="8ab8c-108">Method</span></span>|<span data-ttu-id="8ab8c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8ab8c-109">Return Type</span></span>|<span data-ttu-id="8ab8c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ab8c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8ab8c-111">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="8ab8c-111">Get deviceManagement</span></span>](../api/intune-notification-devicemanagement-get.md)|[<span data-ttu-id="8ab8c-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="8ab8c-112">deviceManagement</span></span>](../resources/intune-notification-devicemanagement.md)|<span data-ttu-id="8ab8c-113">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-notification-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="8ab8c-113">Read properties and relationships of the [deviceManagement](../resources/intune-notification-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="8ab8c-114">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="8ab8c-114">Update deviceManagement</span></span>](../api/intune-notification-devicemanagement-update.md)|[<span data-ttu-id="8ab8c-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="8ab8c-115">deviceManagement</span></span>](../resources/intune-notification-devicemanagement.md)|<span data-ttu-id="8ab8c-116">Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune-notification-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="8ab8c-116">Update the properties of a [deviceManagement](../resources/intune-notification-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8ab8c-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ab8c-117">Properties</span></span>
|<span data-ttu-id="8ab8c-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ab8c-118">Property</span></span>|<span data-ttu-id="8ab8c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ab8c-119">Type</span></span>|<span data-ttu-id="8ab8c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ab8c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ab8c-121">id</span><span class="sxs-lookup"><span data-stu-id="8ab8c-121">id</span></span>|<span data-ttu-id="8ab8c-122">String</span><span class="sxs-lookup"><span data-stu-id="8ab8c-122">String</span></span>|<span data-ttu-id="8ab8c-123">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8ab8c-123">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ab8c-124">Relações</span><span class="sxs-lookup"><span data-stu-id="8ab8c-124">Relationships</span></span>
|<span data-ttu-id="8ab8c-125">Relação</span><span class="sxs-lookup"><span data-stu-id="8ab8c-125">Relationship</span></span>|<span data-ttu-id="8ab8c-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ab8c-126">Type</span></span>|<span data-ttu-id="8ab8c-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ab8c-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ab8c-128">notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="8ab8c-128">notificationMessageTemplates</span></span>|<span data-ttu-id="8ab8c-129">Conjunto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="8ab8c-129">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="8ab8c-130">Os modelos de mensagens de notificação.</span><span class="sxs-lookup"><span data-stu-id="8ab8c-130">The Notification Message Templates.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ab8c-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ab8c-131">JSON Representation</span></span>
<span data-ttu-id="8ab8c-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ab8c-132">Here is a JSON representation of the resource.</span></span>
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




