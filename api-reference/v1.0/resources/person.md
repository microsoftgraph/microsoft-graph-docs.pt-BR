---
title: Tipo de recurso person
description: Uma agregação de informações sobre uma pessoa provenientes de emails, contatos e redes sociais. As pessoas podem ser contatos locais, contatos das redes sociais ou do diretório da sua organização e as pessoas de comunicações recentes (como emails e Skype).
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 27f0f5c27814ff09433cc68b82930878feb95963
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447203"
---
# <a name="person-resource-type"></a><span data-ttu-id="89dde-104">Tipo de recurso person</span><span class="sxs-lookup"><span data-stu-id="89dde-104">person resource type</span></span>

<span data-ttu-id="89dde-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89dde-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89dde-p102">Uma agregação de informações sobre uma pessoa provenientes de emails, contatos e redes sociais. As pessoas podem ser contatos locais, contatos das redes sociais ou do diretório da sua organização e as pessoas de comunicações recentes (como emails e Skype).</span><span class="sxs-lookup"><span data-stu-id="89dde-p102">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="89dde-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="89dde-108">Methods</span></span>

| <span data-ttu-id="89dde-109">Método</span><span class="sxs-lookup"><span data-stu-id="89dde-109">Method</span></span> | <span data-ttu-id="89dde-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="89dde-110">Return Type</span></span> | <span data-ttu-id="89dde-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="89dde-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="89dde-112">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="89dde-112">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="89dde-113">**person**</span><span class="sxs-lookup"><span data-stu-id="89dde-113">**person**</span></span> |<span data-ttu-id="89dde-114">Obtém uma coleção de objetos person ordenados por relevância para o [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="89dde-114">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="89dde-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89dde-115">Properties</span></span>

| <span data-ttu-id="89dde-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89dde-116">Property</span></span> | <span data-ttu-id="89dde-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="89dde-117">Type</span></span> | <span data-ttu-id="89dde-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="89dde-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="89dde-119">birthday</span><span class="sxs-lookup"><span data-stu-id="89dde-119">birthday</span></span>|<span data-ttu-id="89dde-120">String</span><span class="sxs-lookup"><span data-stu-id="89dde-120">String</span></span>|<span data-ttu-id="89dde-121">O aniversário da pessoa.</span><span class="sxs-lookup"><span data-stu-id="89dde-121">The person's birthday.</span></span>|
|<span data-ttu-id="89dde-122">companyName</span><span class="sxs-lookup"><span data-stu-id="89dde-122">companyName</span></span>|<span data-ttu-id="89dde-123">String</span><span class="sxs-lookup"><span data-stu-id="89dde-123">String</span></span>|<span data-ttu-id="89dde-124">O nome da empresa da pessoa.</span><span class="sxs-lookup"><span data-stu-id="89dde-124">The name of the person's company.</span></span>|
|<span data-ttu-id="89dde-125">departamento</span><span class="sxs-lookup"><span data-stu-id="89dde-125">department</span></span>|<span data-ttu-id="89dde-126">String</span><span class="sxs-lookup"><span data-stu-id="89dde-126">String</span></span>|<span data-ttu-id="89dde-127">O departamento da pessoa.</span><span class="sxs-lookup"><span data-stu-id="89dde-127">The person's department.</span></span>|
|<span data-ttu-id="89dde-128">displayName</span><span class="sxs-lookup"><span data-stu-id="89dde-128">displayName</span></span>|<span data-ttu-id="89dde-129">String</span><span class="sxs-lookup"><span data-stu-id="89dde-129">String</span></span>|<span data-ttu-id="89dde-130">O nome de exibição da pessoa.</span><span class="sxs-lookup"><span data-stu-id="89dde-130">The person's display name.</span></span>|
|<span data-ttu-id="89dde-131">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="89dde-131">scoredEmailAddresses</span></span>|<span data-ttu-id="89dde-132">Coleção [scoredEmailAddress](scoredemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="89dde-132">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="89dde-133">Os endereços de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="89dde-133">The person's email addresses.</span></span>|
|<span data-ttu-id="89dde-134">givenName</span><span class="sxs-lookup"><span data-stu-id="89dde-134">givenName</span></span>|<span data-ttu-id="89dde-135">String</span><span class="sxs-lookup"><span data-stu-id="89dde-135">String</span></span>|<span data-ttu-id="89dde-136">O nome fornecido da pessoa.</span><span class="sxs-lookup"><span data-stu-id="89dde-136">The person's given name.</span></span>|
|<span data-ttu-id="89dde-137">id</span><span class="sxs-lookup"><span data-stu-id="89dde-137">id</span></span>|<span data-ttu-id="89dde-138">String</span><span class="sxs-lookup"><span data-stu-id="89dde-138">String</span></span>|<span data-ttu-id="89dde-p103">O identificador exclusivo da pessoa. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="89dde-p103">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="89dde-141">imAddress</span><span class="sxs-lookup"><span data-stu-id="89dde-141">imAddress</span></span>|<span data-ttu-id="89dde-142">String</span><span class="sxs-lookup"><span data-stu-id="89dde-142">String</span></span>|<span data-ttu-id="89dde-p104">O endereço do protocolo SIP (Início de Sessão) de VoIP (Voice over IP) da mensagem instantânea para o usuário. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="89dde-p104">The instant message voice over IP (VOIP) session initiation protocol (SIP) address for the user. Read-only.</span></span>|
|<span data-ttu-id="89dde-145">isFavorite</span><span class="sxs-lookup"><span data-stu-id="89dde-145">isFavorite</span></span>|<span data-ttu-id="89dde-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="89dde-146">Boolean</span></span>|<span data-ttu-id="89dde-147">`true` se o usuário tiver sinalizado essa pessoa como um favorito.</span><span class="sxs-lookup"><span data-stu-id="89dde-147">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="89dde-148">jobTitle</span><span class="sxs-lookup"><span data-stu-id="89dde-148">jobTitle</span></span>|<span data-ttu-id="89dde-149">String</span><span class="sxs-lookup"><span data-stu-id="89dde-149">String</span></span>|<span data-ttu-id="89dde-150">O cargo da pessoa.</span><span class="sxs-lookup"><span data-stu-id="89dde-150">The person's job title.</span></span>|
|<span data-ttu-id="89dde-151">officeLocation</span><span class="sxs-lookup"><span data-stu-id="89dde-151">officeLocation</span></span>|<span data-ttu-id="89dde-152">String</span><span class="sxs-lookup"><span data-stu-id="89dde-152">String</span></span>|<span data-ttu-id="89dde-153">O local do escritório da pessoa.</span><span class="sxs-lookup"><span data-stu-id="89dde-153">The location of the person's office.</span></span>|
|<span data-ttu-id="89dde-154">personNotes</span><span class="sxs-lookup"><span data-stu-id="89dde-154">personNotes</span></span>|<span data-ttu-id="89dde-155">String</span><span class="sxs-lookup"><span data-stu-id="89dde-155">String</span></span>|<span data-ttu-id="89dde-156">As anotações de forma livre que o usuário fez sobre essa pessoa.</span><span class="sxs-lookup"><span data-stu-id="89dde-156">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="89dde-157">personType</span><span class="sxs-lookup"><span data-stu-id="89dde-157">personType</span></span>|[<span data-ttu-id="89dde-158">personType</span><span class="sxs-lookup"><span data-stu-id="89dde-158">personType</span></span>](persontype.md) |<span data-ttu-id="89dde-159">O tipo de pessoa.</span><span class="sxs-lookup"><span data-stu-id="89dde-159">The type of person.</span></span>|
|<span data-ttu-id="89dde-160">telefones</span><span class="sxs-lookup"><span data-stu-id="89dde-160">phones</span></span>|<span data-ttu-id="89dde-161">Coleção [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="89dde-161">[phone](phone.md) collection</span></span>|<span data-ttu-id="89dde-162">Os números de telefone da pessoa.</span><span class="sxs-lookup"><span data-stu-id="89dde-162">The person's phone numbers.</span></span>|
|<span data-ttu-id="89dde-163">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="89dde-163">postalAddresses</span></span>|<span data-ttu-id="89dde-164">[location](location.md) collection</span><span class="sxs-lookup"><span data-stu-id="89dde-164">[location](location.md) collection</span></span>|<span data-ttu-id="89dde-165">Os endereços da pessoa.</span><span class="sxs-lookup"><span data-stu-id="89dde-165">The person's addresses.</span></span>|
|<span data-ttu-id="89dde-166">profession</span><span class="sxs-lookup"><span data-stu-id="89dde-166">profession</span></span>|<span data-ttu-id="89dde-167">String</span><span class="sxs-lookup"><span data-stu-id="89dde-167">String</span></span>|<span data-ttu-id="89dde-168">A profissão da pessoa.</span><span class="sxs-lookup"><span data-stu-id="89dde-168">The person's profession.</span></span>|
|<span data-ttu-id="89dde-169">surname</span><span class="sxs-lookup"><span data-stu-id="89dde-169">surname</span></span>|<span data-ttu-id="89dde-170">String</span><span class="sxs-lookup"><span data-stu-id="89dde-170">String</span></span>|<span data-ttu-id="89dde-171">O sobrenome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="89dde-171">The person's surname.</span></span>|
|<span data-ttu-id="89dde-172">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="89dde-172">userPrincipalName</span></span>|<span data-ttu-id="89dde-173">String</span><span class="sxs-lookup"><span data-stu-id="89dde-173">String</span></span>|<span data-ttu-id="89dde-p105">O nome UPN da pessoa. O UPN é um nome de logon para a pessoa ao estilo da Internet com base na [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email da pessoa. O formato geral é alias@domínio.</span><span class="sxs-lookup"><span data-stu-id="89dde-p105">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="89dde-178">websites</span><span class="sxs-lookup"><span data-stu-id="89dde-178">websites</span></span>|<span data-ttu-id="89dde-179">Coleção [website](website.md)</span><span class="sxs-lookup"><span data-stu-id="89dde-179">[website](website.md) collection</span></span>|<span data-ttu-id="89dde-180">Os sites da pessoa.</span><span class="sxs-lookup"><span data-stu-id="89dde-180">The person's websites.</span></span>|
|<span data-ttu-id="89dde-181">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="89dde-181">yomiCompany</span></span>|<span data-ttu-id="89dde-182">String</span><span class="sxs-lookup"><span data-stu-id="89dde-182">String</span></span>|<span data-ttu-id="89dde-183">O nome japonês fonético da empresa da pessoa.</span><span class="sxs-lookup"><span data-stu-id="89dde-183">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89dde-184">Relações</span><span class="sxs-lookup"><span data-stu-id="89dde-184">Relationships</span></span>

<span data-ttu-id="89dde-185">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89dde-185">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="89dde-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89dde-186">JSON representation</span></span>

<span data-ttu-id="89dde-187">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89dde-187">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "scoredEmailAddresses": [{"@odata.type": "microsoft.graph.scoredEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "imAddress": "string",
  "isFavorite": true,
  "jobTitle": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": {"@odata.type": "microsoft.graph.personType"},
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "surname": "string",
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
