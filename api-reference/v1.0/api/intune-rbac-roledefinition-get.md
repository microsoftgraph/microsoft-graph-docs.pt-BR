---
title: Acessar roleDefinition
description: Leia as propriedades e as relações do objeto roleDefinition.
ms.openlocfilehash: 2a0cf39bf05dda6f427794aa4fd0abc5a007a53f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006582"
---
# <a name="get-roledefinition"></a><span data-ttu-id="937df-103">Acessar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="937df-103">Get roleDefinition</span></span>

> <span data-ttu-id="937df-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="937df-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="937df-105">Leia as propriedades e as relações do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="937df-105">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="937df-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="937df-106">Prerequisites</span></span>
<span data-ttu-id="937df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="937df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="937df-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="937df-109">Permission type</span></span>|<span data-ttu-id="937df-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="937df-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="937df-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="937df-111">Delegated (work or school account)</span></span>|<span data-ttu-id="937df-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="937df-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="937df-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="937df-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="937df-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="937df-114">Not supported.</span></span>|
|<span data-ttu-id="937df-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="937df-115">Application</span></span>|<span data-ttu-id="937df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="937df-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="937df-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="937df-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="937df-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="937df-118">Optional query parameters</span></span>
<span data-ttu-id="937df-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="937df-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="937df-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="937df-120">Request headers</span></span>
|<span data-ttu-id="937df-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="937df-121">Header</span></span>|<span data-ttu-id="937df-122">Valor</span><span class="sxs-lookup"><span data-stu-id="937df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="937df-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="937df-123">Authorization</span></span>|<span data-ttu-id="937df-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="937df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="937df-125">Accept</span><span class="sxs-lookup"><span data-stu-id="937df-125">Accept</span></span>|<span data-ttu-id="937df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="937df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="937df-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="937df-127">Request body</span></span>
<span data-ttu-id="937df-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="937df-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="937df-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="937df-129">Response</span></span>
<span data-ttu-id="937df-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [roleDefinition](../resources/intune-rbac-roledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="937df-130">If successful, this method returns a `200 OK` response code and [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="937df-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="937df-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="937df-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="937df-132">Request</span></span>
<span data-ttu-id="937df-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="937df-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="937df-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="937df-134">Response</span></span>
<span data-ttu-id="937df-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="937df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 690

{
  "value": {
    "@odata.type": "#microsoft.graph.roleDefinition",
    "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
    "displayName": "Display Name value",
    "description": "Description value",
    "rolePermissions": [
      {
        "@odata.type": "microsoft.graph.rolePermission",
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
    ],
    "isBuiltIn": true
  }
}
```



