---
title: Tipo de recurso managedAppStatus
description: Representa o status de proteção e configuração do aplicativo para a organização.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7625543106b1ccf019df9622c1b0f37d40232f0c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415562"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="a20cc-103">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a20cc-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="a20cc-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="a20cc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a20cc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a20cc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a20cc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="a20cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a20cc-107">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="a20cc-107">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="a20cc-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="a20cc-108">Methods</span></span>
|<span data-ttu-id="a20cc-109">Método</span><span class="sxs-lookup"><span data-stu-id="a20cc-109">Method</span></span>|<span data-ttu-id="a20cc-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a20cc-110">Return Type</span></span>|<span data-ttu-id="a20cc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a20cc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a20cc-112">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="a20cc-112">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="a20cc-113">Conjunto [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="a20cc-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="a20cc-114">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a20cc-114">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="a20cc-115">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a20cc-115">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="a20cc-116">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a20cc-116">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="a20cc-117">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a20cc-117">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a20cc-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a20cc-118">Properties</span></span>
|<span data-ttu-id="a20cc-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a20cc-119">Property</span></span>|<span data-ttu-id="a20cc-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a20cc-120">Type</span></span>|<span data-ttu-id="a20cc-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a20cc-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a20cc-122">displayName</span><span class="sxs-lookup"><span data-stu-id="a20cc-122">displayName</span></span>|<span data-ttu-id="a20cc-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a20cc-123">String</span></span>|<span data-ttu-id="a20cc-124">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="a20cc-124">Friendly name of the status report.</span></span>|
|<span data-ttu-id="a20cc-125">id</span><span class="sxs-lookup"><span data-stu-id="a20cc-125">id</span></span>|<span data-ttu-id="a20cc-126">String</span><span class="sxs-lookup"><span data-stu-id="a20cc-126">String</span></span>|<span data-ttu-id="a20cc-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a20cc-127">Key of the entity.</span></span>|
|<span data-ttu-id="a20cc-128">version</span><span class="sxs-lookup"><span data-stu-id="a20cc-128">version</span></span>|<span data-ttu-id="a20cc-129">String</span><span class="sxs-lookup"><span data-stu-id="a20cc-129">String</span></span>|<span data-ttu-id="a20cc-130">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="a20cc-130">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a20cc-131">Relações</span><span class="sxs-lookup"><span data-stu-id="a20cc-131">Relationships</span></span>
<span data-ttu-id="a20cc-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a20cc-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a20cc-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a20cc-133">JSON Representation</span></span>
<span data-ttu-id="a20cc-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a20cc-134">Here is a JSON representation of the resource.</span></span>
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




