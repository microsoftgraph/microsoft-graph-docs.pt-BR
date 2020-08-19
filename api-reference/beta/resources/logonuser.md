---
title: tipo de recurso logonUser
description: Contém informações de estado sobre o usuário conectado neste host
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f480ff8c67c602512d7d8ef3f090366734f0ca7e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808659"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="7d486-103">tipo de recurso logonUser</span><span class="sxs-lookup"><span data-stu-id="7d486-103">logonUser resource type</span></span>

<span data-ttu-id="7d486-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d486-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7d486-105">Contém informações de estado sobre o usuário conectado neste host</span><span class="sxs-lookup"><span data-stu-id="7d486-105">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="7d486-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d486-106">Properties</span></span>

| <span data-ttu-id="7d486-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d486-107">Property</span></span>   | <span data-ttu-id="7d486-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d486-108">Type</span></span> |<span data-ttu-id="7d486-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d486-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d486-110">accountDomain</span><span class="sxs-lookup"><span data-stu-id="7d486-110">accountDomain</span></span>|<span data-ttu-id="7d486-111">String</span><span class="sxs-lookup"><span data-stu-id="7d486-111">String</span></span>|<span data-ttu-id="7d486-112">Domínio da conta de usuário usada para fazer logon.</span><span class="sxs-lookup"><span data-stu-id="7d486-112">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="7d486-113">accountName</span><span class="sxs-lookup"><span data-stu-id="7d486-113">accountName</span></span>|<span data-ttu-id="7d486-114">String</span><span class="sxs-lookup"><span data-stu-id="7d486-114">String</span></span>|<span data-ttu-id="7d486-115">Nome da conta de usuário usada para fazer logon.</span><span class="sxs-lookup"><span data-stu-id="7d486-115">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="7d486-116">accountType</span><span class="sxs-lookup"><span data-stu-id="7d486-116">accountType</span></span>|<span data-ttu-id="7d486-117">String</span><span class="sxs-lookup"><span data-stu-id="7d486-117">String</span></span>|<span data-ttu-id="7d486-118">Tipo de conta de usuário, por definição do Windows.</span><span class="sxs-lookup"><span data-stu-id="7d486-118">User Account type, per Windows definition.</span></span> <span data-ttu-id="7d486-119">Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="7d486-119">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="7d486-120">firstSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="7d486-120">firstSeenDateTime</span></span>|<span data-ttu-id="7d486-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d486-121">DateTimeOffset</span></span>|<span data-ttu-id="7d486-122">Data e hora em que o logon mais antigo por essa conta de usuário ocorreu (período determinado pelo provedor).</span><span class="sxs-lookup"><span data-stu-id="7d486-122">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="7d486-123">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7d486-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7d486-124">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7d486-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7d486-125">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="7d486-125">lastSeenDateTime</span></span>|<span data-ttu-id="7d486-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d486-126">DateTimeOffset</span></span>|<span data-ttu-id="7d486-127">DateTime no qual a conta de usuário tem o logon mais recente.</span><span class="sxs-lookup"><span data-stu-id="7d486-127">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="7d486-128">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7d486-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7d486-129">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7d486-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7d486-130">LogonId</span><span class="sxs-lookup"><span data-stu-id="7d486-130">logonId</span></span>|<span data-ttu-id="7d486-131">String</span><span class="sxs-lookup"><span data-stu-id="7d486-131">String</span></span>|<span data-ttu-id="7d486-132">ID de logon do usuário.</span><span class="sxs-lookup"><span data-stu-id="7d486-132">User logon ID.</span></span>|
|<span data-ttu-id="7d486-133">Logontypesowner</span><span class="sxs-lookup"><span data-stu-id="7d486-133">logonTypes</span></span>|<span data-ttu-id="7d486-134">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d486-134">String collection</span></span>|<span data-ttu-id="7d486-135">Coleção dos tipos de logon observados para o usuário conectado da primeira vez para a última vista.</span><span class="sxs-lookup"><span data-stu-id="7d486-135">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="7d486-136">Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="7d486-136">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d486-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d486-137">JSON representation</span></span>

<span data-ttu-id="7d486-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d486-138">The following is a JSON representation of the resource.</span></span>

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
