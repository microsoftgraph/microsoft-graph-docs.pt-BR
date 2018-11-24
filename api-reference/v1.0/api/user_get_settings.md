# <a name="get-settings"></a><span data-ttu-id="bf522-101">Obter configurações</span><span class="sxs-lookup"><span data-stu-id="bf522-101">Get settings</span></span>

<span data-ttu-id="bf522-102">Leia o objeto de [configurações](../resources/user_settings.md) de usuário e da organização.</span><span class="sxs-lookup"><span data-stu-id="bf522-102">Read the user and organization [settings](../resources/user_settings.md) object.</span></span>
<span data-ttu-id="bf522-103">Para saber como atualizar as propriedades do objeto de [configurações](../resources/user_settings.md) , consulte [Atualizar configurações de usuário](user_update_settings.md).</span><span class="sxs-lookup"><span data-stu-id="bf522-103">To learn how to update the properties of the [settings](../resources/user_settings.md) object, see [update user settings](user_update_settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bf522-104">Permissions</span><span class="sxs-lookup"><span data-stu-id="bf522-104">Permissions</span></span>

<span data-ttu-id="bf522-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bf522-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bf522-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf522-107">Permission type</span></span>      | <span data-ttu-id="bf522-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf522-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf522-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf522-109">Delegated (work or school account)</span></span> | <span data-ttu-id="bf522-110">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf522-110">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="bf522-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf522-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf522-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf522-112">Not supported.</span></span>    |
|<span data-ttu-id="bf522-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf522-113">Application</span></span> | <span data-ttu-id="bf522-114">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf522-114">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf522-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf522-115">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="bf522-116">Solicitar com uma id de usuário' ' ou 'userPrincipalName' só está acessível pelo usuário ou por um usuário com as permissões User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="bf522-116">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="bf522-117">Para saber mais, consulte [Permissions](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bf522-117">To learn more, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="bf522-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf522-118">Request body</span></span>

<span data-ttu-id="bf522-119">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bf522-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf522-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf522-120">Response</span></span>

<span data-ttu-id="bf522-121">Se tiver êxito, este método retornará um `200 OK` objeto de [configurações de usuário](../resources/user_settings.md) e o código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf522-121">If successful, this method returns a `200 OK` response code and [user settings](../resources/user_settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf522-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf522-122">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bf522-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf522-123">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a><span data-ttu-id="bf522-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf522-124">Response</span></span>

<span data-ttu-id="bf522-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bf522-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

