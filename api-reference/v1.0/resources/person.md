# <a name="person-resource-type"></a><span data-ttu-id="a201e-101">Tipo de recurso person</span><span class="sxs-lookup"><span data-stu-id="a201e-101">person resource type</span></span>

<span data-ttu-id="a201e-p101">Uma agregação de informações sobre uma pessoa provenientes de emails, contatos e redes sociais. As pessoas podem ser contatos locais, contatos das redes sociais ou do diretório da sua organização e as pessoas de comunicações recentes (como emails e Skype).</span><span class="sxs-lookup"><span data-stu-id="a201e-p101">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="a201e-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="a201e-104">Methods</span></span>

| <span data-ttu-id="a201e-105">Método</span><span class="sxs-lookup"><span data-stu-id="a201e-105">Method</span></span> | <span data-ttu-id="a201e-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a201e-106">Return Type</span></span> | <span data-ttu-id="a201e-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="a201e-107">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="a201e-108">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="a201e-108">List people</span></span>](../api/user_list_people.md) | <span data-ttu-id="a201e-109">**person**</span><span class="sxs-lookup"><span data-stu-id="a201e-109">**person**</span></span> |<span data-ttu-id="a201e-110">Obtém uma coleção de objetos person ordenados por relevância para o [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="a201e-110">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="a201e-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a201e-111">Properties</span></span>

| <span data-ttu-id="a201e-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a201e-112">Property</span></span> | <span data-ttu-id="a201e-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="a201e-113">Type</span></span> | <span data-ttu-id="a201e-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="a201e-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a201e-115">birthday</span><span class="sxs-lookup"><span data-stu-id="a201e-115">birthday</span></span>|<span data-ttu-id="a201e-116">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="a201e-116">String</span></span>|<span data-ttu-id="a201e-117">O aniversário da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a201e-117">The person's birthday.</span></span>|
|<span data-ttu-id="a201e-118">companyName</span><span class="sxs-lookup"><span data-stu-id="a201e-118">companyName</span></span>|<span data-ttu-id="a201e-119">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="a201e-119">String</span></span>|<span data-ttu-id="a201e-120">O nome da empresa da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a201e-120">The name of the person's company.</span></span>|
|<span data-ttu-id="a201e-121">departamento</span><span class="sxs-lookup"><span data-stu-id="a201e-121">department</span></span>|<span data-ttu-id="a201e-122">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="a201e-122">String</span></span>|<span data-ttu-id="a201e-123">O departamento da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a201e-123">The person's department.</span></span>|
|<span data-ttu-id="a201e-124">displayName</span><span class="sxs-lookup"><span data-stu-id="a201e-124">displayName</span></span>|<span data-ttu-id="a201e-125">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="a201e-125">String</span></span>|<span data-ttu-id="a201e-126">O nome de exibição da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a201e-126">The person's display name.</span></span>|
|<span data-ttu-id="a201e-127">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="a201e-127">scoredEmailAddresses</span></span>|<span data-ttu-id="a201e-128">Coleção [scoredEmailAddress](scoredemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="a201e-128">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="a201e-129">Os endereços de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a201e-129">The person's email addresses.</span></span>|
|<span data-ttu-id="a201e-130">givenName</span><span class="sxs-lookup"><span data-stu-id="a201e-130">givenName</span></span>|<span data-ttu-id="a201e-131">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="a201e-131">String</span></span>|<span data-ttu-id="a201e-132">O nome fornecido da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a201e-132">The person's given name.</span></span>|
|<span data-ttu-id="a201e-133">id</span><span class="sxs-lookup"><span data-stu-id="a201e-133">id</span></span>|<span data-ttu-id="a201e-134">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="a201e-134">String</span></span>|<span data-ttu-id="a201e-p102">O identificador exclusivo da pessoa. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a201e-p102">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="a201e-137">imAddress</span><span class="sxs-lookup"><span data-stu-id="a201e-137">imAddress</span></span>|<span data-ttu-id="a201e-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a201e-138">String</span></span>|<span data-ttu-id="a201e-p103">O endereço do protocolo SIP (Início de Sessão) de VoIP (Voice over IP) da mensagem instantânea para o usuário. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a201e-p103">The instant message voice over IP (VOIP) session initiation protocol (SIP) address for the user. Read-only.</span></span>|
|<span data-ttu-id="a201e-141">isFavorite</span><span class="sxs-lookup"><span data-stu-id="a201e-141">isFavorite</span></span>|<span data-ttu-id="a201e-142">Booleano</span><span class="sxs-lookup"><span data-stu-id="a201e-142">Boolean</span></span>|<span data-ttu-id="a201e-143">`true` se o usuário tiver sinalizado essa pessoa como um favorito.</span><span class="sxs-lookup"><span data-stu-id="a201e-143">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="a201e-144">jobTitle</span><span class="sxs-lookup"><span data-stu-id="a201e-144">jobTitle</span></span>|<span data-ttu-id="a201e-145">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="a201e-145">String</span></span>|<span data-ttu-id="a201e-146">O cargo da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a201e-146">The person's job title.</span></span>|
|<span data-ttu-id="a201e-147">officeLocation</span><span class="sxs-lookup"><span data-stu-id="a201e-147">officeLocation</span></span>|<span data-ttu-id="a201e-148">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="a201e-148">String</span></span>|<span data-ttu-id="a201e-149">O local do escritório da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a201e-149">The location of the person's office.</span></span>|
|<span data-ttu-id="a201e-150">personNotes</span><span class="sxs-lookup"><span data-stu-id="a201e-150">personNotes</span></span>|<span data-ttu-id="a201e-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a201e-151">String</span></span>|<span data-ttu-id="a201e-152">As anotações de forma livre que o usuário fez sobre essa pessoa.</span><span class="sxs-lookup"><span data-stu-id="a201e-152">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="a201e-153">personType</span><span class="sxs-lookup"><span data-stu-id="a201e-153">personType</span></span>|[<span data-ttu-id="a201e-154">personType</span><span class="sxs-lookup"><span data-stu-id="a201e-154">personType</span></span>](persontype.md) |<span data-ttu-id="a201e-155">O tipo de pessoa.</span><span class="sxs-lookup"><span data-stu-id="a201e-155">The type of person.</span></span>|
|<span data-ttu-id="a201e-156">telefones</span><span class="sxs-lookup"><span data-stu-id="a201e-156">phones</span></span>|<span data-ttu-id="a201e-157">Coleção [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="a201e-157">[phone](phone.md) collection</span></span>|<span data-ttu-id="a201e-158">Os números de telefone da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a201e-158">The person's phone numbers.</span></span>|
|<span data-ttu-id="a201e-159">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="a201e-159">postalAddresses</span></span>|<span data-ttu-id="a201e-160">Coleção [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="a201e-160">[location](location.md) collection</span></span>|<span data-ttu-id="a201e-161">Os endereços da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a201e-161">The person's addresses.</span></span>|
|<span data-ttu-id="a201e-162">profession</span><span class="sxs-lookup"><span data-stu-id="a201e-162">profession</span></span>|<span data-ttu-id="a201e-163">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="a201e-163">String</span></span>|<span data-ttu-id="a201e-164">A profissão da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a201e-164">The person's profession.</span></span>|
|<span data-ttu-id="a201e-165">surname</span><span class="sxs-lookup"><span data-stu-id="a201e-165">surname</span></span>|<span data-ttu-id="a201e-166">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="a201e-166">String</span></span>|<span data-ttu-id="a201e-167">O sobrenome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a201e-167">The person's surname.</span></span>|
|<span data-ttu-id="a201e-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a201e-168">userPrincipalName</span></span>|<span data-ttu-id="a201e-169">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="a201e-169">String</span></span>|<span data-ttu-id="a201e-p104">O nome UPN da pessoa. O UPN é um nome de logon para a pessoa ao estilo da Internet com base na [RFC 822](http://www.ietf.org/rfc/rfc0822.txt) padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email da pessoa. O formato geral é alias@domínio.</span><span class="sxs-lookup"><span data-stu-id="a201e-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](http://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="a201e-174">websites</span><span class="sxs-lookup"><span data-stu-id="a201e-174">websites</span></span>|<span data-ttu-id="a201e-175">Coleção [website](website.md)</span><span class="sxs-lookup"><span data-stu-id="a201e-175">[website](website.md) collection</span></span>|<span data-ttu-id="a201e-176">Os sites da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a201e-176">The person's websites.</span></span>|
|<span data-ttu-id="a201e-177">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="a201e-177">yomiCompany</span></span>|<span data-ttu-id="a201e-178">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="a201e-178">String</span></span>|<span data-ttu-id="a201e-179">O nome japonês fonético da empresa da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a201e-179">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a201e-180">Relações</span><span class="sxs-lookup"><span data-stu-id="a201e-180">Relationships</span></span>

<span data-ttu-id="a201e-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a201e-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a201e-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a201e-182">JSON representation</span></span>

<span data-ttu-id="a201e-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a201e-183">The following is a JSON representation of the resource.</span></span>

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
