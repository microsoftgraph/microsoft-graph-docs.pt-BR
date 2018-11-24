# <a name="geteffectivepermissions-function"></a><span data-ttu-id="498b0-101">Função getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="498b0-101">getEffectivePermissions function</span></span>

> <span data-ttu-id="498b0-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="498b0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="498b0-103">Recupera permissões efetivas de usuário autenticado no momento</span><span class="sxs-lookup"><span data-stu-id="498b0-103">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="498b0-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="498b0-104">Prerequisites</span></span>
<span data-ttu-id="498b0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="498b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="498b0-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="498b0-107">Permission type</span></span>|<span data-ttu-id="498b0-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="498b0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="498b0-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="498b0-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="498b0-110">&nbsp;&nbsp; Controle de acesso baseado em função</span><span class="sxs-lookup"><span data-stu-id="498b0-110">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="498b0-111">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="498b0-111">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="498b0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="498b0-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="498b0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="498b0-113">Not supported.</span></span>|
|<span data-ttu-id="498b0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="498b0-114">Application</span></span>|<span data-ttu-id="498b0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="498b0-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="498b0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="498b0-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="498b0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="498b0-117">Request headers</span></span>
|<span data-ttu-id="498b0-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="498b0-118">Header</span></span>|<span data-ttu-id="498b0-119">Valor</span><span class="sxs-lookup"><span data-stu-id="498b0-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="498b0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="498b0-120">Authorization</span></span>|<span data-ttu-id="498b0-121">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="498b0-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="498b0-122">Accept</span><span class="sxs-lookup"><span data-stu-id="498b0-122">Accept</span></span>|<span data-ttu-id="498b0-123">application/json</span><span class="sxs-lookup"><span data-stu-id="498b0-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="498b0-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="498b0-124">Request body</span></span>
<span data-ttu-id="498b0-125">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="498b0-125">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="498b0-126">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="498b0-126">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="498b0-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="498b0-127">Property</span></span>|<span data-ttu-id="498b0-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="498b0-128">Type</span></span>|<span data-ttu-id="498b0-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="498b0-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="498b0-130">scope</span><span class="sxs-lookup"><span data-stu-id="498b0-130">scope</span></span>|<span data-ttu-id="498b0-131">String</span><span class="sxs-lookup"><span data-stu-id="498b0-131">String</span></span>|<span data-ttu-id="498b0-132">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="498b0-132">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="498b0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="498b0-133">Response</span></span>
<span data-ttu-id="498b0-134">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [rolePermission](../resources/intune_rbac_rolepermission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="498b0-134">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune_rbac_rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="498b0-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="498b0-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="498b0-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="498b0-136">Request</span></span>
<span data-ttu-id="498b0-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="498b0-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="498b0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="498b0-138">Response</span></span>
<span data-ttu-id="498b0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="498b0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "value": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ]
}
```



