---
title: Tipo de recurso managedAppStatus
description: Representa o status de proteção e configuração do aplicativo para a organização.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac7e2c727bce9da64e9262e3e3165a0bcc024623
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923709"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="0b92b-103">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="0b92b-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="0b92b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0b92b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b92b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0b92b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b92b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0b92b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b92b-107">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="0b92b-107">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="0b92b-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="0b92b-108">Methods</span></span>
|<span data-ttu-id="0b92b-109">Método</span><span class="sxs-lookup"><span data-stu-id="0b92b-109">Method</span></span>|<span data-ttu-id="0b92b-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0b92b-110">Return Type</span></span>|<span data-ttu-id="0b92b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b92b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0b92b-112">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="0b92b-112">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="0b92b-113">Conjunto [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="0b92b-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="0b92b-114">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="0b92b-114">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="0b92b-115">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="0b92b-115">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="0b92b-116">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="0b92b-116">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="0b92b-117">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="0b92b-117">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b92b-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b92b-118">Properties</span></span>
|<span data-ttu-id="0b92b-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b92b-119">Property</span></span>|<span data-ttu-id="0b92b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b92b-120">Type</span></span>|<span data-ttu-id="0b92b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b92b-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b92b-122">displayName</span><span class="sxs-lookup"><span data-stu-id="0b92b-122">displayName</span></span>|<span data-ttu-id="0b92b-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b92b-123">String</span></span>|<span data-ttu-id="0b92b-124">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="0b92b-124">Friendly name of the status report.</span></span>|
|<span data-ttu-id="0b92b-125">id</span><span class="sxs-lookup"><span data-stu-id="0b92b-125">id</span></span>|<span data-ttu-id="0b92b-126">String</span><span class="sxs-lookup"><span data-stu-id="0b92b-126">String</span></span>|<span data-ttu-id="0b92b-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0b92b-127">Key of the entity.</span></span>|
|<span data-ttu-id="0b92b-128">version</span><span class="sxs-lookup"><span data-stu-id="0b92b-128">version</span></span>|<span data-ttu-id="0b92b-129">String</span><span class="sxs-lookup"><span data-stu-id="0b92b-129">String</span></span>|<span data-ttu-id="0b92b-130">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="0b92b-130">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b92b-131">Relações</span><span class="sxs-lookup"><span data-stu-id="0b92b-131">Relationships</span></span>
<span data-ttu-id="0b92b-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b92b-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0b92b-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b92b-133">JSON Representation</span></span>
<span data-ttu-id="0b92b-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b92b-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```





