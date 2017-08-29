# <a name="person-resource-type"></a><span data-ttu-id="214ea-101">Tipo de recurso person</span><span class="sxs-lookup"><span data-stu-id="214ea-101">person resource type</span></span>

<span data-ttu-id="214ea-p101">Uma agregação de informações sobre uma pessoa provenientes de emails, contatos e redes sociais. As pessoas podem ser contatos locais, contatos das redes sociais ou do diretório da sua organização e as pessoas de comunicações recentes (como emails e Skype).</span><span class="sxs-lookup"><span data-stu-id="214ea-p101">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="214ea-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="214ea-104">Methods</span></span>

| <span data-ttu-id="214ea-105">Método</span><span class="sxs-lookup"><span data-stu-id="214ea-105">Method</span></span>           | <span data-ttu-id="214ea-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="214ea-106">Return Type</span></span>    |<span data-ttu-id="214ea-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="214ea-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="214ea-108">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="214ea-108">List people</span></span>](../api/user_list_people.md) | <span data-ttu-id="214ea-109">**person**</span><span class="sxs-lookup"><span data-stu-id="214ea-109">**person**</span></span> |<span data-ttu-id="214ea-110">Obtém uma coleção de objetos person ordenados por relevância para o [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="214ea-110">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|
|[<span data-ttu-id="214ea-111">Obter person</span><span class="sxs-lookup"><span data-stu-id="214ea-111">Get person</span></span>](../api/person_get.md) | <span data-ttu-id="214ea-112">**person**</span><span class="sxs-lookup"><span data-stu-id="214ea-112">**person**</span></span> |<span data-ttu-id="214ea-113">Obter as propriedades e os relacionamentos de um objeto person.</span><span class="sxs-lookup"><span data-stu-id="214ea-113">Get properties and relationships of a person object.</span></span>|

## <a name="properties"></a><span data-ttu-id="214ea-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="214ea-114">Properties</span></span>
| <span data-ttu-id="214ea-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="214ea-115">Property</span></span>     | <span data-ttu-id="214ea-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="214ea-116">Type</span></span>   |<span data-ttu-id="214ea-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="214ea-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="214ea-118">birthday</span><span class="sxs-lookup"><span data-stu-id="214ea-118">birthday</span></span>|<span data-ttu-id="214ea-119">String</span><span class="sxs-lookup"><span data-stu-id="214ea-119">String</span></span>|<span data-ttu-id="214ea-120">O aniversário da pessoa.</span><span class="sxs-lookup"><span data-stu-id="214ea-120">The person's birthday.</span></span>|
|<span data-ttu-id="214ea-121">companyName</span><span class="sxs-lookup"><span data-stu-id="214ea-121">companyName</span></span>|<span data-ttu-id="214ea-122">String</span><span class="sxs-lookup"><span data-stu-id="214ea-122">String</span></span>|<span data-ttu-id="214ea-123">O nome da empresa da pessoa.</span><span class="sxs-lookup"><span data-stu-id="214ea-123">The name of the person's company.</span></span>|
|<span data-ttu-id="214ea-124">departamento</span><span class="sxs-lookup"><span data-stu-id="214ea-124">department</span></span>|<span data-ttu-id="214ea-125">String</span><span class="sxs-lookup"><span data-stu-id="214ea-125">String</span></span>|<span data-ttu-id="214ea-126">O departamento da pessoa.</span><span class="sxs-lookup"><span data-stu-id="214ea-126">The person's department.</span></span>|
|<span data-ttu-id="214ea-127">displayName</span><span class="sxs-lookup"><span data-stu-id="214ea-127">displayName</span></span>|<span data-ttu-id="214ea-128">String</span><span class="sxs-lookup"><span data-stu-id="214ea-128">String</span></span>|<span data-ttu-id="214ea-129">O nome de exibição da pessoa.</span><span class="sxs-lookup"><span data-stu-id="214ea-129">The person's display name.</span></span>|
|<span data-ttu-id="214ea-130">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="214ea-130">scoredEmailAddresses</span></span>|<span data-ttu-id="214ea-131">Coleção [scoredEmailAddress](scoredemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="214ea-131">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="214ea-132">Os endereços de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="214ea-132">The person's email addresses.</span></span>|
|<span data-ttu-id="214ea-133">givenName</span><span class="sxs-lookup"><span data-stu-id="214ea-133">givenName</span></span>|<span data-ttu-id="214ea-134">String</span><span class="sxs-lookup"><span data-stu-id="214ea-134">String</span></span>|<span data-ttu-id="214ea-135">O nome fornecido da pessoa.</span><span class="sxs-lookup"><span data-stu-id="214ea-135">The person's given name.</span></span>|
|<span data-ttu-id="214ea-136">id</span><span class="sxs-lookup"><span data-stu-id="214ea-136">id</span></span>|<span data-ttu-id="214ea-137">String</span><span class="sxs-lookup"><span data-stu-id="214ea-137">String</span></span>|<span data-ttu-id="214ea-p102">O identificador exclusivo da pessoa. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="214ea-p102">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="214ea-140">imAddress</span><span class="sxs-lookup"><span data-stu-id="214ea-140">imAddress</span></span>|<span data-ttu-id="214ea-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="214ea-141">String collection</span></span>|<span data-ttu-id="214ea-p103">O endereço do protocolo SIP (Início de Sessão) de VoIP (Voice over IP) da mensagem instantânea para o usuário. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="214ea-p103">The instant message voice over IP (VOIP) session initiation protocol (SIP) address for the user. Read-only.</span></span>|
|<span data-ttu-id="214ea-144">isFavorite</span><span class="sxs-lookup"><span data-stu-id="214ea-144">isFavorite</span></span>|<span data-ttu-id="214ea-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="214ea-145">Boolean</span></span>|<span data-ttu-id="214ea-146">`true` se o usuário tiver sinalizado essa pessoa como um favorito.</span><span class="sxs-lookup"><span data-stu-id="214ea-146">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="214ea-147">jobTitle</span><span class="sxs-lookup"><span data-stu-id="214ea-147">jobTitle</span></span>|<span data-ttu-id="214ea-148">String</span><span class="sxs-lookup"><span data-stu-id="214ea-148">String</span></span>|<span data-ttu-id="214ea-149">O cargo da pessoa.</span><span class="sxs-lookup"><span data-stu-id="214ea-149">The person's job title.</span></span>|
|<span data-ttu-id="214ea-150">officeLocation</span><span class="sxs-lookup"><span data-stu-id="214ea-150">officeLocation</span></span>|<span data-ttu-id="214ea-151">String</span><span class="sxs-lookup"><span data-stu-id="214ea-151">String</span></span>|<span data-ttu-id="214ea-152">O local do escritório da pessoa.</span><span class="sxs-lookup"><span data-stu-id="214ea-152">The location of the person's office.</span></span>|
|<span data-ttu-id="214ea-153">personNotes</span><span class="sxs-lookup"><span data-stu-id="214ea-153">personNotes</span></span>|<span data-ttu-id="214ea-154">String</span><span class="sxs-lookup"><span data-stu-id="214ea-154">String</span></span>|<span data-ttu-id="214ea-155">Anotações de forma livre que o usuário fez sobre essa pessoa.</span><span class="sxs-lookup"><span data-stu-id="214ea-155">Free-form notes that the the user has taken about this person.</span></span>|
|<span data-ttu-id="214ea-156">personType</span><span class="sxs-lookup"><span data-stu-id="214ea-156">personType</span></span>|<span data-ttu-id="214ea-157">Coleção [personType](persontype.md)</span><span class="sxs-lookup"><span data-stu-id="214ea-157">[personType](persontype.md) collection</span></span>|<span data-ttu-id="214ea-158">O tipo de pessoa.</span><span class="sxs-lookup"><span data-stu-id="214ea-158">The type of person.</span></span>|
|<span data-ttu-id="214ea-159">telefones</span><span class="sxs-lookup"><span data-stu-id="214ea-159">phones</span></span>|<span data-ttu-id="214ea-160">Coleção [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="214ea-160">[phone](phone.md) collection</span></span>|<span data-ttu-id="214ea-161">Os números de telefone da pessoa.</span><span class="sxs-lookup"><span data-stu-id="214ea-161">The person's phone numbers.</span></span>|
|<span data-ttu-id="214ea-162">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="214ea-162">postalAddresses</span></span>|<span data-ttu-id="214ea-163">[location](location.md) collection</span><span class="sxs-lookup"><span data-stu-id="214ea-163">[location](location.md) collection</span></span>|<span data-ttu-id="214ea-164">Os endereços da pessoa.</span><span class="sxs-lookup"><span data-stu-id="214ea-164">The person's addresses.</span></span>|
|<span data-ttu-id="214ea-165">profession</span><span class="sxs-lookup"><span data-stu-id="214ea-165">profession</span></span>|<span data-ttu-id="214ea-166">String</span><span class="sxs-lookup"><span data-stu-id="214ea-166">String</span></span>|<span data-ttu-id="214ea-167">A profissão da pessoa.</span><span class="sxs-lookup"><span data-stu-id="214ea-167">The person's profession.</span></span>|
|<span data-ttu-id="214ea-168">surname</span><span class="sxs-lookup"><span data-stu-id="214ea-168">surname</span></span>|<span data-ttu-id="214ea-169">String</span><span class="sxs-lookup"><span data-stu-id="214ea-169">String</span></span>|<span data-ttu-id="214ea-170">O sobrenome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="214ea-170">The person's surname.</span></span>|
|<span data-ttu-id="214ea-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="214ea-171">userPrincipalName</span></span>|<span data-ttu-id="214ea-172">String</span><span class="sxs-lookup"><span data-stu-id="214ea-172">String</span></span>|<span data-ttu-id="214ea-p104">O nome UPN da pessoa. O UPN é um nome de logon para a pessoa ao estilo da Internet com base na [RFC 822](http://www.ietf.org/rfc/rfc0822.txt) padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email da pessoa. O formato geral é alias@domínio.</span><span class="sxs-lookup"><span data-stu-id="214ea-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](http://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="214ea-177">websites</span><span class="sxs-lookup"><span data-stu-id="214ea-177">websites</span></span>|<span data-ttu-id="214ea-178">Coleção [website](website.md)</span><span class="sxs-lookup"><span data-stu-id="214ea-178">[website](website.md) collection</span></span>|<span data-ttu-id="214ea-179">Os sites da pessoa.</span><span class="sxs-lookup"><span data-stu-id="214ea-179">The person's websites.</span></span>|
|<span data-ttu-id="214ea-180">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="214ea-180">yomiCompany</span></span>|<span data-ttu-id="214ea-181">String</span><span class="sxs-lookup"><span data-stu-id="214ea-181">String</span></span>|<span data-ttu-id="214ea-182">O nome japonês fonético da empresa da pessoa.</span><span class="sxs-lookup"><span data-stu-id="214ea-182">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="214ea-183">Relações</span><span class="sxs-lookup"><span data-stu-id="214ea-183">Relationships</span></span>
<span data-ttu-id="214ea-184">Nenhum</span><span class="sxs-lookup"><span data-stu-id="214ea-184">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="214ea-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="214ea-185">JSON representation</span></span>

<span data-ttu-id="214ea-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="214ea-186">The following is a JSON representation of the resource.</span></span>

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
  "scoredEmailAddresses": [{"@odata.type": "microsoft.graph.scoredemailaddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "isFavorite": true,
  "jobTitle": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": [{"@odata.type": "microsoft.graph.persontype"}],
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
