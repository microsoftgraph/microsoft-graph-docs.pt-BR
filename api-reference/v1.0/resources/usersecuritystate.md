# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="f81bf-101">tipo de recurso de userSecurityState</span><span class="sxs-lookup"><span data-stu-id="f81bf-101">userSecurityState resource type</span></span>

<span data-ttu-id="f81bf-102">Contém informações com estado sobre a conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="f81bf-102">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="f81bf-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f81bf-103">Properties</span></span>

| <span data-ttu-id="f81bf-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f81bf-104">Property</span></span>   | <span data-ttu-id="f81bf-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="f81bf-105">Type</span></span> |<span data-ttu-id="f81bf-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="f81bf-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f81bf-107">aadUserId</span><span class="sxs-lookup"><span data-stu-id="f81bf-107">aadUserId</span></span>|<span data-ttu-id="f81bf-108">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f81bf-108">String</span></span>|<span data-ttu-id="f81bf-109">Identificador de Objeto do Usuário AAD (GUID) - representa a entidade de usuário física/de várias contas.</span><span class="sxs-lookup"><span data-stu-id="f81bf-109">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="f81bf-110">accountName</span><span class="sxs-lookup"><span data-stu-id="f81bf-110">accountName</span></span>|<span data-ttu-id="f81bf-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f81bf-111">String</span></span>|<span data-ttu-id="f81bf-112">Nome da conta de usuário (sem o domínio do Active Directory ou domínio DNS) - conta (também chamado de `mailNickName`).</span><span class="sxs-lookup"><span data-stu-id="f81bf-112">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="f81bf-113">domainName</span><span class="sxs-lookup"><span data-stu-id="f81bf-113">domainName</span></span>|<span data-ttu-id="f81bf-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f81bf-114">String</span></span>|<span data-ttu-id="f81bf-115">Domínio NetBIOS/Active Directory da conta de usuário (ou seja, no formato domínio\conta).</span><span class="sxs-lookup"><span data-stu-id="f81bf-115">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="f81bf-116">emailRole</span><span class="sxs-lookup"><span data-stu-id="f81bf-116">emailRole</span></span>|<span data-ttu-id="f81bf-117">emailRole</span><span class="sxs-lookup"><span data-stu-id="f81bf-117">emailRole</span></span>|<span data-ttu-id="f81bf-118">Para alertas relacionados a e-mail - 'função' do e-mail da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="f81bf-118">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="f81bf-119">Os valores possíveis são: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="f81bf-119">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="f81bf-120">isVpn</span><span class="sxs-lookup"><span data-stu-id="f81bf-120">isVpn</span></span>|<span data-ttu-id="f81bf-121">Booleano</span><span class="sxs-lookup"><span data-stu-id="f81bf-121">Boolean</span></span>|<span data-ttu-id="f81bf-122">Indica se o usuário efetuou logon por meio de uma VPN.</span><span class="sxs-lookup"><span data-stu-id="f81bf-122">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="f81bf-123">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="f81bf-123">logonDateTime</span></span>|<span data-ttu-id="f81bf-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f81bf-124">DateTimeOffset</span></span>|<span data-ttu-id="f81bf-125">Hora em que o login ocorreu.</span><span class="sxs-lookup"><span data-stu-id="f81bf-125">Time at which the sign-in occurred.</span></span> <span data-ttu-id="f81bf-126">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f81bf-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f81bf-127">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f81bf-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f81bf-128">identificação de logon</span><span class="sxs-lookup"><span data-stu-id="f81bf-128">logonId</span></span>|<span data-ttu-id="f81bf-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f81bf-129">String</span></span>|<span data-ttu-id="f81bf-130">ID de login do usuário.</span><span class="sxs-lookup"><span data-stu-id="f81bf-130">User sign-in ID.</span></span>|
|<span data-ttu-id="f81bf-131">logonIp</span><span class="sxs-lookup"><span data-stu-id="f81bf-131">logonIp</span></span>|<span data-ttu-id="f81bf-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f81bf-132">String</span></span>|<span data-ttu-id="f81bf-133">Endereço IP onde foi originada a solicitação de login.</span><span class="sxs-lookup"><span data-stu-id="f81bf-133">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="f81bf-134">logonLocation</span><span class="sxs-lookup"><span data-stu-id="f81bf-134">logonLocation</span></span>|<span data-ttu-id="f81bf-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f81bf-135">String</span></span>|<span data-ttu-id="f81bf-136">Local (por um mapeamento de endereço IP) associado a um evento de entrada do usuário por esse usuário.</span><span class="sxs-lookup"><span data-stu-id="f81bf-136">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="f81bf-137">logonType</span><span class="sxs-lookup"><span data-stu-id="f81bf-137">logonType</span></span>|<span data-ttu-id="f81bf-138">logonType</span><span class="sxs-lookup"><span data-stu-id="f81bf-138">logonType</span></span>|<span data-ttu-id="f81bf-139">Método de login do usuário.</span><span class="sxs-lookup"><span data-stu-id="f81bf-139">Method of user sign in.</span></span> <span data-ttu-id="f81bf-140">Os valores possíveis são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="f81bf-140">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="f81bf-141">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="f81bf-141">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="f81bf-142">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="f81bf-142">String</span></span>|<span data-ttu-id="f81bf-143">Identificador de segurança (SID) do Active Directory (no local) do usuário.</span><span class="sxs-lookup"><span data-stu-id="f81bf-143">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="f81bf-144">riskScore</span><span class="sxs-lookup"><span data-stu-id="f81bf-144">riskScore</span></span>|<span data-ttu-id="f81bf-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f81bf-145">String</span></span>|<span data-ttu-id="f81bf-146">Pontuação de risco calculada/gerada pelo provedor da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="f81bf-146">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="f81bf-147">Intervalo de valor recomendado de 0-1, que equivale a um percentual.</span><span class="sxs-lookup"><span data-stu-id="f81bf-147">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="f81bf-148">userAccountType</span><span class="sxs-lookup"><span data-stu-id="f81bf-148">userAccountType</span></span>|<span data-ttu-id="f81bf-149">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="f81bf-149">userAccountSecurityType</span></span>|<span data-ttu-id="f81bf-150">Tipo de conta de usuário (membros do grupo), por definição do Windows.</span><span class="sxs-lookup"><span data-stu-id="f81bf-150">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="f81bf-151">Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="f81bf-151">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="f81bf-152">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f81bf-152">userPrincipalName</span></span>|<span data-ttu-id="f81bf-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f81bf-153">String</span></span>|<span data-ttu-id="f81bf-154">Nome de login do usuário - formato da internet: (nome da conta de usuário)@(nome de domínio DNS da conta de usuário).</span><span class="sxs-lookup"><span data-stu-id="f81bf-154">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f81bf-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f81bf-155">JSON representation</span></span>

<span data-ttu-id="f81bf-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f81bf-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSecurityState"
}-->

```json
{
  "aadUserId": "String",
  "accountName": "String",
  "domainName": "String",
  "emailRole": "@odata.type: microsoft.graph.emailRole",
  "isVpn": true,
  "logonDateTime": "String (timestamp)",
  "logonId": "String",
  "logonIp": "String",
  "logonLocation": "String",
  "logonType": "@odata.type: microsoft.graph.logonType",
  "onPremisesSecurityIdentifier": "String",
  "riskScore": "String",
  "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
