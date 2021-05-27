---
title: Trabalhando com a API de conectores
description: Visão geral da API de conectores do Microsoft Graph
author: mecampos
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 63e11b086592a46a4e519a2ab7c79c20d049213a
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645774"
---
# <a name="working-with-the-connectors-api"></a><span data-ttu-id="19b22-103">Trabalhando com a API de conectores</span><span class="sxs-lookup"><span data-stu-id="19b22-103">Working with the connectors API</span></span>

<span data-ttu-id="19b22-104">Os conectores do Microsoft Graph oferecem uma maneira simples de trazer dados externos para o Microsoft Graph e aprimorar as experiências inteligentes do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="19b22-104">Microsoft Graph connectors offer a simple way to bring external data into Microsoft Graph and enhance Microsoft 365 intelligent experiences.</span></span> <span data-ttu-id="19b22-105">Você pode criar um conector personalizado para integração com serviços que não estão disponíveis como conectores desenvolvidos pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="19b22-105">You might want to build a custom connector to integrate with services that aren't available as connectors built by Microsoft.</span></span> <span data-ttu-id="19b22-106">Para criar conectores personalizados, use as APIs REST do conector do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="19b22-106">To build custom connectors, you use the Microsoft Graph connector REST APIs.</span></span>

![Imagem mostrando os dados externos chegando através de diferentes tipos de conectores para o Microsoft Graph](./images/connectors-images/api-overview.png)

<span data-ttu-id="19b22-108">Você pode usar a API de conectores do Microsoft Graph para:</span><span class="sxs-lookup"><span data-stu-id="19b22-108">You can use the Microsoft Graph connectors API to:</span></span>

1. <span data-ttu-id="19b22-109">Criar e gerenciar conexões de dados externos.</span><span class="sxs-lookup"><span data-stu-id="19b22-109">Create and manage external data connections.</span></span>
2. <span data-ttu-id="19b22-110">Definir e registrar o esquema dos tipos de dados externos.</span><span class="sxs-lookup"><span data-stu-id="19b22-110">Define and register the schema of the external data type(s).</span></span>
3. <span data-ttu-id="19b22-111">Ingerir itens de dados externos no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="19b22-111">Ingest external data items into Microsoft Graph.</span></span>
4. <span data-ttu-id="19b22-112">Sincronizar grupos externos.</span><span class="sxs-lookup"><span data-stu-id="19b22-112">Sync external groups.</span></span>

<span data-ttu-id="19b22-113">Para obter mais detalhes sobre essas APIs, confira a documentação sugerida a seguir.</span><span class="sxs-lookup"><span data-stu-id="19b22-113">To learn more details about these APIs, you can visit the documentation suggested next.</span></span>

## <a name="connections-api"></a><span data-ttu-id="19b22-114">API de conexões</span><span class="sxs-lookup"><span data-stu-id="19b22-114">Connections API</span></span>

<span data-ttu-id="19b22-115">Uma conexão é um contêiner lógico dos dados externos que você pode gerenciar como uma única unidade.</span><span class="sxs-lookup"><span data-stu-id="19b22-115">A connection is a logical container for your external data that you can manage as a single unit.</span></span>
<span data-ttu-id="19b22-116">Para saber mais sobre como criar, atualizar e excluir conexões no Microsoft Graph, visite a seção [Gerenciar conexão](connecting-external-content-manage-connections.md).</span><span class="sxs-lookup"><span data-stu-id="19b22-116">To learn more about how to create, update, and delete connections in the Microsoft Graph, visit the [Manage connection](connecting-external-content-manage-connections.md) section.</span></span>

## <a name="schema-api"></a><span data-ttu-id="19b22-117">API de esquema</span><span class="sxs-lookup"><span data-stu-id="19b22-117">Schema API</span></span>

<span data-ttu-id="19b22-118">O [esquema](/graph/api/resources/schema?view=graph-rest-beta&amp;preserve-view=true) de conexão determina como seu conteúdo será usado em várias experiências do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="19b22-118">The connection [schema](/graph/api/resources/schema?view=graph-rest-beta&amp;preserve-view=true) determines how your content will be used in various Microsoft 365 experiences.</span></span> <span data-ttu-id="19b22-119">O esquema é uma lista simples de todas as propriedades que você planeja adicionar à conexão junto com seus atributos, rótulos e aliases.</span><span class="sxs-lookup"><span data-stu-id="19b22-119">Schema is a flat list of all the properties you plan to add to the connection along with their attributes, labels, and aliases.</span></span> <span data-ttu-id="19b22-120">Você deve registrar o esquema antes de ingerir itens no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="19b22-120">You must register the schema before ingesting items into Microsoft Graph.</span></span>

<span data-ttu-id="19b22-121">Para saber mais sobre como registrar o esquema da conexão do Microsoft Graph e suas propriedades, visite a seção [Gerenciar esquema](connecting-external-content-manage-schema.md).</span><span class="sxs-lookup"><span data-stu-id="19b22-121">To learn more about how to register the schema for the Microsoft Graph connection, and its properties, visit the [Manage schema](connecting-external-content-manage-schema.md) section.</span></span>

## <a name="ingest-external-data-items"></a><span data-ttu-id="19b22-122">Ingerir itens de dados externos</span><span class="sxs-lookup"><span data-stu-id="19b22-122">Ingest external data items</span></span>

<span data-ttu-id="19b22-123">Os conectores do Microsoft Graph oferecem uma maneira simples de trazer dados externos para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="19b22-123">Microsoft Graph connectors offer a simple way to bring external data into Microsoft Graph.</span></span> <span data-ttu-id="19b22-124">Os itens adicionados por seu aplicativo ao serviço Pesquisa da Microsoft são representados pelo recurso [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="19b22-124">Items added by your application to the Microsoft Search service are represented by the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) resource in Microsoft Graph.</span></span>

<span data-ttu-id="19b22-125">Para saber mais sobre como criar, atualizar e excluir itens adicionados por seu aplicativo por meio de conectores do Microsoft Graph, visite a seção [Gerenciar itens](connecting-external-content-manage-items.md).</span><span class="sxs-lookup"><span data-stu-id="19b22-125">To learn more about how to create, update, and delete items added by your application via Microsoft Graph connectors, visit the [Manage items](connecting-external-content-manage-items.md) section.</span></span>

## <a name="external-groups-api"></a><span data-ttu-id="19b22-126">API de grupos externos</span><span class="sxs-lookup"><span data-stu-id="19b22-126">External groups API</span></span>

<span data-ttu-id="19b22-127">Os itens no serviço externo podem ter acesso concedido ou negado por meio da ACL para diferentes tipos de grupos que não são do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="19b22-127">Items in the external service can be granted or denied access via ACL to different types of non-Azure Active Directory groups.</span></span> <span data-ttu-id="19b22-128">Por exemplo, os itens do Salesforce podem ter perfis e conjuntos de permissões.</span><span class="sxs-lookup"><span data-stu-id="19b22-128">For example, Salesforce items might have permission sets and profiles.</span></span> <span data-ttu-id="19b22-129">Os itens do ServiceNow podem ter grupos locais.</span><span class="sxs-lookup"><span data-stu-id="19b22-129">ServiceNow items might have local groups.</span></span> <span data-ttu-id="19b22-130">Ao ingerir esses itens no Microsoft Graph, você precisará respeitar essas ACLs.</span><span class="sxs-lookup"><span data-stu-id="19b22-130">When you ingest these items into Microsoft Graph, you need to honor these ACLs.</span></span>

<span data-ttu-id="19b22-131">Você pode usar a API de grupos externos para definir permissões sobre itens externos ingeridos no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="19b22-131">You can use the External groups API to set permissions on external items ingested into Microsoft Graph.</span></span> <span data-ttu-id="19b22-132">Um [externalGroup](/graph/api/externalgroup-post-members?view=graph-rest-beta&amp;preserve-view=true) representa uma construção semelhante a um grupo ou um grupo que não faz parte do Azure Active Directory (como unidades de negócios, equipes e assim por diante) e determina as permissões no conteúdo em sua fonte de dados externa.</span><span class="sxs-lookup"><span data-stu-id="19b22-132">An [externalGroup](/graph/api/externalgroup-post-members?view=graph-rest-beta&amp;preserve-view=true) represents a non-Azure Active Directory group or group-like construct (such as Business units, Teams, and so on) and determines permissions on the content in your external data source.</span></span>