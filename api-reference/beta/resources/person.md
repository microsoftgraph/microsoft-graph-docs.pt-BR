---
title: Tipo de recurso person
description: Uma agregação de informações sobre uma pessoa através de email, contatos e redes sociais. As pessoas podem ser contatos locais, contatos de redes sociais, diretório da sua organização e pessoas de comunicações recentes (como email e Skype).
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 32a2c9905ab52e9b229bb8673fb4a84d90a706ac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561471"
---
# <a name="person-resource-type"></a><span data-ttu-id="a4974-104">Tipo de recurso person</span><span class="sxs-lookup"><span data-stu-id="a4974-104">person resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4974-105">Uma agregação de informações sobre uma pessoa através de email, contatos e redes sociais.</span><span class="sxs-lookup"><span data-stu-id="a4974-105">An aggregation of information about a person from across mail, contacts and social networks.</span></span> <span data-ttu-id="a4974-106">As pessoas podem ser contatos locais, contatos de redes sociais, diretório da sua organização e pessoas de comunicações recentes (como email e Skype).</span><span class="sxs-lookup"><span data-stu-id="a4974-106">People can be local contacts, contacts from social networking, your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="a4974-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a4974-107">Methods</span></span>

| <span data-ttu-id="a4974-108">Método</span><span class="sxs-lookup"><span data-stu-id="a4974-108">Method</span></span> | <span data-ttu-id="a4974-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a4974-109">Return Type</span></span> | <span data-ttu-id="a4974-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4974-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="a4974-111">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="a4974-111">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="a4974-112">**person**</span><span class="sxs-lookup"><span data-stu-id="a4974-112">**person**</span></span> |<span data-ttu-id="a4974-113">Obtém uma coleção de objetos person ordenados por relevância para o [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="a4974-113">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="a4974-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4974-114">Properties</span></span>

| <span data-ttu-id="a4974-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4974-115">Property</span></span> | <span data-ttu-id="a4974-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4974-116">Type</span></span> | <span data-ttu-id="a4974-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4974-117">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a4974-118">birthday</span><span class="sxs-lookup"><span data-stu-id="a4974-118">birthday</span></span>|<span data-ttu-id="a4974-119">string</span><span class="sxs-lookup"><span data-stu-id="a4974-119">string</span></span>|<span data-ttu-id="a4974-120">O aniversário da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4974-120">The person's birthday.</span></span>|
|<span data-ttu-id="a4974-121">companyName</span><span class="sxs-lookup"><span data-stu-id="a4974-121">companyName</span></span>|<span data-ttu-id="a4974-122">string</span><span class="sxs-lookup"><span data-stu-id="a4974-122">string</span></span>|<span data-ttu-id="a4974-123">O nome da empresa da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4974-123">The name of the person's company.</span></span>|
|<span data-ttu-id="a4974-124">departamento</span><span class="sxs-lookup"><span data-stu-id="a4974-124">department</span></span>|<span data-ttu-id="a4974-125">string</span><span class="sxs-lookup"><span data-stu-id="a4974-125">string</span></span>|<span data-ttu-id="a4974-126">O departamento da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4974-126">The person's department.</span></span>|
|<span data-ttu-id="a4974-127">displayName</span><span class="sxs-lookup"><span data-stu-id="a4974-127">displayName</span></span>|<span data-ttu-id="a4974-128">string</span><span class="sxs-lookup"><span data-stu-id="a4974-128">string</span></span>|<span data-ttu-id="a4974-129">O nome de exibição da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4974-129">The person's display name.</span></span>|
|<span data-ttu-id="a4974-130">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="a4974-130">emailAddresses</span></span>|<span data-ttu-id="a4974-131">coleção [rankedEmailAddress](rankedemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="a4974-131">[rankedEmailAddress](rankedemailaddress.md) collection</span></span>|<span data-ttu-id="a4974-132">Os endereços de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4974-132">The person's email addresses.</span></span>|
|<span data-ttu-id="a4974-133">givenName</span><span class="sxs-lookup"><span data-stu-id="a4974-133">givenName</span></span>|<span data-ttu-id="a4974-134">string</span><span class="sxs-lookup"><span data-stu-id="a4974-134">string</span></span>|<span data-ttu-id="a4974-135">O nome fornecido da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4974-135">The person's given name.</span></span>|
|<span data-ttu-id="a4974-136">id</span><span class="sxs-lookup"><span data-stu-id="a4974-136">id</span></span>|<span data-ttu-id="a4974-137">string</span><span class="sxs-lookup"><span data-stu-id="a4974-137">string</span></span>|<span data-ttu-id="a4974-138">O identificador exclusivo da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4974-138">The person's unique identifier.</span></span> <span data-ttu-id="a4974-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a4974-139">Read-only.</span></span>|
|<span data-ttu-id="a4974-140">isFavorite</span><span class="sxs-lookup"><span data-stu-id="a4974-140">isFavorite</span></span>|<span data-ttu-id="a4974-141">booliano</span><span class="sxs-lookup"><span data-stu-id="a4974-141">boolean</span></span>|<span data-ttu-id="a4974-142">`true` se o usuário tiver sinalizado essa pessoa como um favorito.</span><span class="sxs-lookup"><span data-stu-id="a4974-142">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="a4974-143">mailboxType</span><span class="sxs-lookup"><span data-stu-id="a4974-143">mailboxType</span></span>|<span data-ttu-id="a4974-144">string</span><span class="sxs-lookup"><span data-stu-id="a4974-144">string</span></span>|<span data-ttu-id="a4974-145">O tipo de caixa de correio que é representado pelo endereço de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4974-145">The type of mailbox that is represented by the person's email address.</span></span>|
|<span data-ttu-id="a4974-146">officeLocation</span><span class="sxs-lookup"><span data-stu-id="a4974-146">officeLocation</span></span>|<span data-ttu-id="a4974-147">string</span><span class="sxs-lookup"><span data-stu-id="a4974-147">string</span></span>|<span data-ttu-id="a4974-148">O local do escritório da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4974-148">The location of the person's office.</span></span>|
|<span data-ttu-id="a4974-149">personNotes</span><span class="sxs-lookup"><span data-stu-id="a4974-149">personNotes</span></span>|<span data-ttu-id="a4974-150">string</span><span class="sxs-lookup"><span data-stu-id="a4974-150">string</span></span>|<span data-ttu-id="a4974-151">As anotações de forma livre que o usuário fez sobre essa pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4974-151">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="a4974-152">personType</span><span class="sxs-lookup"><span data-stu-id="a4974-152">personType</span></span>|<span data-ttu-id="a4974-153">string</span><span class="sxs-lookup"><span data-stu-id="a4974-153">string</span></span>|<span data-ttu-id="a4974-154">O tipo de pessoa, por exemplo, lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="a4974-154">The type of person, for example distribution list.</span></span>|
|<span data-ttu-id="a4974-155">telefones</span><span class="sxs-lookup"><span data-stu-id="a4974-155">phones</span></span>|<span data-ttu-id="a4974-156">Coleção [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="a4974-156">[phone](phone.md) collection</span></span>|<span data-ttu-id="a4974-157">Os números de telefone da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4974-157">The person's phone numbers.</span></span>|
|<span data-ttu-id="a4974-158">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="a4974-158">postalAddresses</span></span>|<span data-ttu-id="a4974-159">[location](location.md) collection</span><span class="sxs-lookup"><span data-stu-id="a4974-159">[location](location.md) collection</span></span>|<span data-ttu-id="a4974-160">Os endereços da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4974-160">The person's addresses.</span></span>|
|<span data-ttu-id="a4974-161">profession</span><span class="sxs-lookup"><span data-stu-id="a4974-161">profession</span></span>|<span data-ttu-id="a4974-162">string</span><span class="sxs-lookup"><span data-stu-id="a4974-162">string</span></span>|<span data-ttu-id="a4974-163">A profissão da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4974-163">The person's profession.</span></span>|
|<span data-ttu-id="a4974-164">fontes</span><span class="sxs-lookup"><span data-stu-id="a4974-164">sources</span></span>|<span data-ttu-id="a4974-165">coleção [personDataSource](persondatasource.md)</span><span class="sxs-lookup"><span data-stu-id="a4974-165">[personDataSource](persondatasource.md) collection</span></span>|<span data-ttu-id="a4974-166">As fontes das quais os dados do usuário são provenientes, por exemplo, contatos do Outlook ou do Outlook.</span><span class="sxs-lookup"><span data-stu-id="a4974-166">The sources the user data comes from, for example Directory or Outlook Contacts.</span></span>|
|<span data-ttu-id="a4974-167">surname</span><span class="sxs-lookup"><span data-stu-id="a4974-167">surname</span></span>|<span data-ttu-id="a4974-168">string</span><span class="sxs-lookup"><span data-stu-id="a4974-168">string</span></span>|<span data-ttu-id="a4974-169">O sobrenome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4974-169">The person's surname.</span></span>|
|<span data-ttu-id="a4974-170">title</span><span class="sxs-lookup"><span data-stu-id="a4974-170">title</span></span>|<span data-ttu-id="a4974-171">string</span><span class="sxs-lookup"><span data-stu-id="a4974-171">string</span></span>|<span data-ttu-id="a4974-172">O título da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4974-172">The person's title.</span></span>|
|<span data-ttu-id="a4974-173">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a4974-173">userPrincipalName</span></span>|<span data-ttu-id="a4974-174">string</span><span class="sxs-lookup"><span data-stu-id="a4974-174">string</span></span>|<span data-ttu-id="a4974-p104">O nome UPN da pessoa. O UPN é um nome de logon para a pessoa ao estilo da Internet com base na [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email da pessoa. O formato geral é alias@domínio.</span><span class="sxs-lookup"><span data-stu-id="a4974-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="a4974-179">websites</span><span class="sxs-lookup"><span data-stu-id="a4974-179">websites</span></span>|<span data-ttu-id="a4974-180">Coleção [website](website.md)</span><span class="sxs-lookup"><span data-stu-id="a4974-180">[website](website.md) collection</span></span>|<span data-ttu-id="a4974-181">Os sites da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4974-181">The person's websites.</span></span>|
|<span data-ttu-id="a4974-182">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="a4974-182">yomiCompany</span></span>|<span data-ttu-id="a4974-183">string</span><span class="sxs-lookup"><span data-stu-id="a4974-183">string</span></span>|<span data-ttu-id="a4974-184">O nome japonês fonético da empresa da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4974-184">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4974-185">Relações</span><span class="sxs-lookup"><span data-stu-id="a4974-185">Relationships</span></span>

<span data-ttu-id="a4974-186">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a4974-186">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4974-187">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4974-187">JSON representation</span></span>

<span data-ttu-id="a4974-188">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a4974-188">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
