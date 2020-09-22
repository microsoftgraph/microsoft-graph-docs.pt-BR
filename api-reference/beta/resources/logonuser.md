---
title: tipo de recurso logonUser
description: Contém informações de estado sobre o usuário conectado neste host
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 737a3ad71ee34641dd6d2c719a7a1975d3fb11ae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075522"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="55adb-103">tipo de recurso logonUser</span><span class="sxs-lookup"><span data-stu-id="55adb-103">logonUser resource type</span></span>

<span data-ttu-id="55adb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55adb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="55adb-105">Contém informações de estado sobre o usuário conectado neste host</span><span class="sxs-lookup"><span data-stu-id="55adb-105">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="55adb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55adb-106">Properties</span></span>

| <span data-ttu-id="55adb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55adb-107">Property</span></span>   | <span data-ttu-id="55adb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="55adb-108">Type</span></span> |<span data-ttu-id="55adb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="55adb-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55adb-110">accountDomain</span><span class="sxs-lookup"><span data-stu-id="55adb-110">accountDomain</span></span>|<span data-ttu-id="55adb-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55adb-111">String</span></span>|<span data-ttu-id="55adb-112">Domínio da conta de usuário usada para fazer logon.</span><span class="sxs-lookup"><span data-stu-id="55adb-112">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="55adb-113">accountName</span><span class="sxs-lookup"><span data-stu-id="55adb-113">accountName</span></span>|<span data-ttu-id="55adb-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55adb-114">String</span></span>|<span data-ttu-id="55adb-115">Nome da conta de usuário usada para fazer logon.</span><span class="sxs-lookup"><span data-stu-id="55adb-115">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="55adb-116">accountType</span><span class="sxs-lookup"><span data-stu-id="55adb-116">accountType</span></span>|<span data-ttu-id="55adb-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55adb-117">String</span></span>|<span data-ttu-id="55adb-118">Tipo de conta de usuário, por definição do Windows.</span><span class="sxs-lookup"><span data-stu-id="55adb-118">User Account type, per Windows definition.</span></span> <span data-ttu-id="55adb-119">Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="55adb-119">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="55adb-120">firstSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="55adb-120">firstSeenDateTime</span></span>|<span data-ttu-id="55adb-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55adb-121">DateTimeOffset</span></span>|<span data-ttu-id="55adb-122">Data e hora em que o logon mais antigo por essa conta de usuário ocorreu (período determinado pelo provedor).</span><span class="sxs-lookup"><span data-stu-id="55adb-122">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="55adb-123">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="55adb-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="55adb-124">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="55adb-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="55adb-125">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="55adb-125">lastSeenDateTime</span></span>|<span data-ttu-id="55adb-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55adb-126">DateTimeOffset</span></span>|<span data-ttu-id="55adb-127">DateTime no qual a conta de usuário tem o logon mais recente.</span><span class="sxs-lookup"><span data-stu-id="55adb-127">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="55adb-128">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="55adb-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="55adb-129">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="55adb-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="55adb-130">LogonId</span><span class="sxs-lookup"><span data-stu-id="55adb-130">logonId</span></span>|<span data-ttu-id="55adb-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55adb-131">String</span></span>|<span data-ttu-id="55adb-132">ID de logon do usuário.</span><span class="sxs-lookup"><span data-stu-id="55adb-132">User logon ID.</span></span>|
|<span data-ttu-id="55adb-133">Logontypesowner</span><span class="sxs-lookup"><span data-stu-id="55adb-133">logonTypes</span></span>|<span data-ttu-id="55adb-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="55adb-134">String collection</span></span>|<span data-ttu-id="55adb-135">Coleção dos tipos de logon observados para o usuário conectado da primeira vez para a última vista.</span><span class="sxs-lookup"><span data-stu-id="55adb-135">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="55adb-136">Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="55adb-136">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55adb-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55adb-137">JSON representation</span></span>

<span data-ttu-id="55adb-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55adb-138">The following is a JSON representation of the resource.</span></span>

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


