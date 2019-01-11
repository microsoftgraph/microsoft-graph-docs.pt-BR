---
title: Tipo de recurso person
description: Uma agregação de informações sobre uma pessoa em email, contatos e redes sociais. Pessoas podem ser contatos locais, contatos de redes sociais, diretório da sua organização e pessoas de comunicações recentes (por exemplo, email e Skype).
author: simonhult
localization_priority: Normal
ms.openlocfilehash: c0318986b01704501a2b7910888d6a5e962a5dca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865377"
---
# <a name="person-resource-type"></a><span data-ttu-id="a4cc2-104">Tipo de recurso person</span><span class="sxs-lookup"><span data-stu-id="a4cc2-104">person resource type</span></span>

> <span data-ttu-id="a4cc2-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4cc2-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4cc2-107">Uma agregação de informações sobre uma pessoa em email, contatos e redes sociais.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-107">An aggregation of information about a person from across mail, contacts and social networks.</span></span> <span data-ttu-id="a4cc2-108">Pessoas podem ser contatos locais, contatos de redes sociais, diretório da sua organização e pessoas de comunicações recentes (por exemplo, email e Skype).</span><span class="sxs-lookup"><span data-stu-id="a4cc2-108">People can be local contacts, contacts from social networking, your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="a4cc2-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="a4cc2-109">Methods</span></span>

| <span data-ttu-id="a4cc2-110">Método</span><span class="sxs-lookup"><span data-stu-id="a4cc2-110">Method</span></span> | <span data-ttu-id="a4cc2-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a4cc2-111">Return Type</span></span> | <span data-ttu-id="a4cc2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4cc2-112">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="a4cc2-113">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="a4cc2-113">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="a4cc2-114">**person**</span><span class="sxs-lookup"><span data-stu-id="a4cc2-114">**person**</span></span> |<span data-ttu-id="a4cc2-115">Obtém uma coleção de objetos person ordenados por relevância para o [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="a4cc2-115">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="a4cc2-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4cc2-116">Properties</span></span>

| <span data-ttu-id="a4cc2-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4cc2-117">Property</span></span> | <span data-ttu-id="a4cc2-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4cc2-118">Type</span></span> | <span data-ttu-id="a4cc2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4cc2-119">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a4cc2-120">birthday</span><span class="sxs-lookup"><span data-stu-id="a4cc2-120">birthday</span></span>|<span data-ttu-id="a4cc2-121">string</span><span class="sxs-lookup"><span data-stu-id="a4cc2-121">string</span></span>|<span data-ttu-id="a4cc2-122">O aniversário da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-122">The person's birthday.</span></span>|
|<span data-ttu-id="a4cc2-123">companyName</span><span class="sxs-lookup"><span data-stu-id="a4cc2-123">companyName</span></span>|<span data-ttu-id="a4cc2-124">string</span><span class="sxs-lookup"><span data-stu-id="a4cc2-124">string</span></span>|<span data-ttu-id="a4cc2-125">O nome da empresa da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-125">The name of the person's company.</span></span>|
|<span data-ttu-id="a4cc2-126">departamento</span><span class="sxs-lookup"><span data-stu-id="a4cc2-126">department</span></span>|<span data-ttu-id="a4cc2-127">string</span><span class="sxs-lookup"><span data-stu-id="a4cc2-127">string</span></span>|<span data-ttu-id="a4cc2-128">O departamento da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-128">The person's department.</span></span>|
|<span data-ttu-id="a4cc2-129">displayName</span><span class="sxs-lookup"><span data-stu-id="a4cc2-129">displayName</span></span>|<span data-ttu-id="a4cc2-130">string</span><span class="sxs-lookup"><span data-stu-id="a4cc2-130">string</span></span>|<span data-ttu-id="a4cc2-131">O nome de exibição da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-131">The person's display name.</span></span>|
|<span data-ttu-id="a4cc2-132">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="a4cc2-132">emailAddresses</span></span>|<span data-ttu-id="a4cc2-133">coleção [rankedEmailAddress](rankedemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="a4cc2-133">[rankedEmailAddress](rankedemailaddress.md) collection</span></span>|<span data-ttu-id="a4cc2-134">Os endereços de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-134">The person's email addresses.</span></span>|
|<span data-ttu-id="a4cc2-135">givenName</span><span class="sxs-lookup"><span data-stu-id="a4cc2-135">givenName</span></span>|<span data-ttu-id="a4cc2-136">string</span><span class="sxs-lookup"><span data-stu-id="a4cc2-136">string</span></span>|<span data-ttu-id="a4cc2-137">O nome fornecido da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-137">The person's given name.</span></span>|
|<span data-ttu-id="a4cc2-138">id</span><span class="sxs-lookup"><span data-stu-id="a4cc2-138">id</span></span>|<span data-ttu-id="a4cc2-139">string</span><span class="sxs-lookup"><span data-stu-id="a4cc2-139">string</span></span>|<span data-ttu-id="a4cc2-p104">O identificador exclusivo da pessoa. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-p104">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="a4cc2-142">isFavorite</span><span class="sxs-lookup"><span data-stu-id="a4cc2-142">isFavorite</span></span>|<span data-ttu-id="a4cc2-143">booliano</span><span class="sxs-lookup"><span data-stu-id="a4cc2-143">boolean</span></span>|<span data-ttu-id="a4cc2-144">`true` se o usuário tiver sinalizado essa pessoa como um favorito.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-144">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="a4cc2-145">mailboxType</span><span class="sxs-lookup"><span data-stu-id="a4cc2-145">mailboxType</span></span>|<span data-ttu-id="a4cc2-146">string</span><span class="sxs-lookup"><span data-stu-id="a4cc2-146">string</span></span>|<span data-ttu-id="a4cc2-147">O tipo de caixa de correio que é representado por um endereço de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-147">The type of mailbox that is represented by the person's email address.</span></span>|
|<span data-ttu-id="a4cc2-148">officeLocation</span><span class="sxs-lookup"><span data-stu-id="a4cc2-148">officeLocation</span></span>|<span data-ttu-id="a4cc2-149">string</span><span class="sxs-lookup"><span data-stu-id="a4cc2-149">string</span></span>|<span data-ttu-id="a4cc2-150">O local do escritório da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-150">The location of the person's office.</span></span>|
|<span data-ttu-id="a4cc2-151">personNotes</span><span class="sxs-lookup"><span data-stu-id="a4cc2-151">personNotes</span></span>|<span data-ttu-id="a4cc2-152">string</span><span class="sxs-lookup"><span data-stu-id="a4cc2-152">string</span></span>|<span data-ttu-id="a4cc2-153">As anotações de forma livre que o usuário fez sobre essa pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-153">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="a4cc2-154">personType</span><span class="sxs-lookup"><span data-stu-id="a4cc2-154">personType</span></span>|<span data-ttu-id="a4cc2-155">string</span><span class="sxs-lookup"><span data-stu-id="a4cc2-155">string</span></span>|<span data-ttu-id="a4cc2-156">O tipo da pessoa, por exemplo lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-156">The type of person, for example distribution list.</span></span>|
|<span data-ttu-id="a4cc2-157">telefones</span><span class="sxs-lookup"><span data-stu-id="a4cc2-157">phones</span></span>|<span data-ttu-id="a4cc2-158">Coleção [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="a4cc2-158">[phone](phone.md) collection</span></span>|<span data-ttu-id="a4cc2-159">Os números de telefone da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-159">The person's phone numbers.</span></span>|
|<span data-ttu-id="a4cc2-160">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="a4cc2-160">postalAddresses</span></span>|<span data-ttu-id="a4cc2-161">[location](location.md) collection</span><span class="sxs-lookup"><span data-stu-id="a4cc2-161">[location](location.md) collection</span></span>|<span data-ttu-id="a4cc2-162">Os endereços da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-162">The person's addresses.</span></span>|
|<span data-ttu-id="a4cc2-163">profession</span><span class="sxs-lookup"><span data-stu-id="a4cc2-163">profession</span></span>|<span data-ttu-id="a4cc2-164">string</span><span class="sxs-lookup"><span data-stu-id="a4cc2-164">string</span></span>|<span data-ttu-id="a4cc2-165">A profissão da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-165">The person's profession.</span></span>|
|<span data-ttu-id="a4cc2-166">sources</span><span class="sxs-lookup"><span data-stu-id="a4cc2-166">sources</span></span>|<span data-ttu-id="a4cc2-167">coleção [personDataSource](persondatasource.md)</span><span class="sxs-lookup"><span data-stu-id="a4cc2-167">[personDataSource](persondatasource.md) collection</span></span>|<span data-ttu-id="a4cc2-168">As fontes de dados do usuário provêm, por exemplo, diretório ou contatos do Outlook.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-168">The sources the user data comes from, for example Directory or Outlook Contacts.</span></span>|
|<span data-ttu-id="a4cc2-169">surname</span><span class="sxs-lookup"><span data-stu-id="a4cc2-169">surname</span></span>|<span data-ttu-id="a4cc2-170">string</span><span class="sxs-lookup"><span data-stu-id="a4cc2-170">string</span></span>|<span data-ttu-id="a4cc2-171">O sobrenome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-171">The person's surname.</span></span>|
|<span data-ttu-id="a4cc2-172">título</span><span class="sxs-lookup"><span data-stu-id="a4cc2-172">title</span></span>|<span data-ttu-id="a4cc2-173">string</span><span class="sxs-lookup"><span data-stu-id="a4cc2-173">string</span></span>|<span data-ttu-id="a4cc2-174">Título da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-174">The person's title.</span></span>|
|<span data-ttu-id="a4cc2-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a4cc2-175">userPrincipalName</span></span>|<span data-ttu-id="a4cc2-176">string</span><span class="sxs-lookup"><span data-stu-id="a4cc2-176">string</span></span>|<span data-ttu-id="a4cc2-p105">O nome UPN da pessoa. O UPN é um nome de logon para a pessoa ao estilo da Internet com base na [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email da pessoa. O formato geral é alias@domínio.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-p105">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="a4cc2-181">websites</span><span class="sxs-lookup"><span data-stu-id="a4cc2-181">websites</span></span>|<span data-ttu-id="a4cc2-182">Coleção [website](website.md)</span><span class="sxs-lookup"><span data-stu-id="a4cc2-182">[website](website.md) collection</span></span>|<span data-ttu-id="a4cc2-183">Os sites da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-183">The person's websites.</span></span>|
|<span data-ttu-id="a4cc2-184">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="a4cc2-184">yomiCompany</span></span>|<span data-ttu-id="a4cc2-185">string</span><span class="sxs-lookup"><span data-stu-id="a4cc2-185">string</span></span>|<span data-ttu-id="a4cc2-186">O nome japonês fonético da empresa da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-186">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4cc2-187">Relações</span><span class="sxs-lookup"><span data-stu-id="a4cc2-187">Relationships</span></span>

<span data-ttu-id="a4cc2-188">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a4cc2-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4cc2-189">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4cc2-189">JSON representation</span></span>

<span data-ttu-id="a4cc2-190">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a4cc2-190">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.rankedEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "isFavorite": true,
  "mailboxType": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "sources": [{"@odata.type": "microsoft.graph.personDataSource"}],
  "surname": "string",
  "title": "string",
  "userPrincipalName": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "yomiCompany": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
