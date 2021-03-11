---
title: Tipo de recurso logonUser
description: Contém informações de estado sobre o usuário conectado neste host
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 9986aaa7cb5fbf5f8687c43de019b234a4a971d8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720491"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="d48fc-103">Tipo de recurso logonUser</span><span class="sxs-lookup"><span data-stu-id="d48fc-103">logonUser resource type</span></span>

<span data-ttu-id="d48fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d48fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d48fc-105">Contém informações de estado sobre o usuário conectado neste host</span><span class="sxs-lookup"><span data-stu-id="d48fc-105">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="d48fc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d48fc-106">Properties</span></span>

| <span data-ttu-id="d48fc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d48fc-107">Property</span></span>   | <span data-ttu-id="d48fc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d48fc-108">Type</span></span> |<span data-ttu-id="d48fc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d48fc-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d48fc-110">accountDomain</span><span class="sxs-lookup"><span data-stu-id="d48fc-110">accountDomain</span></span>|<span data-ttu-id="d48fc-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d48fc-111">String</span></span>|<span data-ttu-id="d48fc-112">Domínio da conta de usuário usada para fazer logon.</span><span class="sxs-lookup"><span data-stu-id="d48fc-112">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="d48fc-113">accountName</span><span class="sxs-lookup"><span data-stu-id="d48fc-113">accountName</span></span>|<span data-ttu-id="d48fc-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d48fc-114">String</span></span>|<span data-ttu-id="d48fc-115">Nome da conta de usuário usada para fazer logon.</span><span class="sxs-lookup"><span data-stu-id="d48fc-115">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="d48fc-116">accountType</span><span class="sxs-lookup"><span data-stu-id="d48fc-116">accountType</span></span>|<span data-ttu-id="d48fc-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d48fc-117">String</span></span>|<span data-ttu-id="d48fc-118">Tipo de Conta de Usuário, por definição do Windows.</span><span class="sxs-lookup"><span data-stu-id="d48fc-118">User Account type, per Windows definition.</span></span> <span data-ttu-id="d48fc-119">Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="d48fc-119">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="d48fc-120">firstSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="d48fc-120">firstSeenDateTime</span></span>|<span data-ttu-id="d48fc-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d48fc-121">DateTimeOffset</span></span>|<span data-ttu-id="d48fc-122">DateTime no qual ocorreu o primeiro logon por essa conta de usuário (período determinado pelo provedor).</span><span class="sxs-lookup"><span data-stu-id="d48fc-122">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="d48fc-123">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d48fc-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d48fc-124">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="d48fc-124">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="d48fc-125">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="d48fc-125">lastSeenDateTime</span></span>|<span data-ttu-id="d48fc-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d48fc-126">DateTimeOffset</span></span>|<span data-ttu-id="d48fc-127">DateTime no qual ocorreu o logon mais recente por essa conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="d48fc-127">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="d48fc-128">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d48fc-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d48fc-129">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="d48fc-129">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="d48fc-130">logonId</span><span class="sxs-lookup"><span data-stu-id="d48fc-130">logonId</span></span>|<span data-ttu-id="d48fc-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d48fc-131">String</span></span>|<span data-ttu-id="d48fc-132">ID de logon do usuário.</span><span class="sxs-lookup"><span data-stu-id="d48fc-132">User logon ID.</span></span>|
|<span data-ttu-id="d48fc-133">logonTypes</span><span class="sxs-lookup"><span data-stu-id="d48fc-133">logonTypes</span></span>|<span data-ttu-id="d48fc-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d48fc-134">String collection</span></span>|<span data-ttu-id="d48fc-135">Coleção dos tipos de logon observados para o usuário conectado de quando foi visto pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="d48fc-135">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="d48fc-136">Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="d48fc-136">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d48fc-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d48fc-137">JSON representation</span></span>

<span data-ttu-id="d48fc-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d48fc-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.logonUser"
}-->

```json
{
  "accountDomain": "String",
  "accountName": "String",
  "accountType": "String",
  "firstSeenDateTime": "String (timestamp)",
  "lastSeenDateTime": "String (timestamp)",
  "logonId": "String",
  "logonTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "logonUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


