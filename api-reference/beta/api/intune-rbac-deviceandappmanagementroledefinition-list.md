---
title: Listar deviceAndAppManagementRoleDefinitions
description: Lista propriedades e relações dos objetos deviceAndAppManagementRoleDefinition.
ms.openlocfilehash: 649e30ead236f83b2364cc242ba9b68796a2fd57
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037936"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="9b830-103">Listar deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="9b830-103">List deviceAndAppManagementRoleDefinitions</span></span>

> <span data-ttu-id="9b830-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9b830-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b830-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9b830-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b830-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9b830-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b830-107">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9b830-107">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b830-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9b830-108">Prerequisites</span></span>
<span data-ttu-id="9b830-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b830-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b830-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b830-111">Permission type</span></span>|<span data-ttu-id="9b830-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9b830-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b830-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b830-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b830-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b830-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="9b830-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b830-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b830-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b830-116">Not supported.</span></span>|
|<span data-ttu-id="9b830-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b830-117">Application</span></span>|<span data-ttu-id="9b830-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b830-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b830-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b830-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="9b830-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b830-120">Request headers</span></span>
|<span data-ttu-id="9b830-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9b830-121">Header</span></span>|<span data-ttu-id="9b830-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9b830-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b830-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b830-123">Authorization</span></span>|<span data-ttu-id="9b830-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b830-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b830-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9b830-125">Accept</span></span>|<span data-ttu-id="9b830-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b830-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b830-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b830-127">Request body</span></span>
<span data-ttu-id="9b830-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b830-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b830-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b830-129">Response</span></span>
<span data-ttu-id="9b830-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b830-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b830-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b830-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b830-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b830-132">Request</span></span>
<span data-ttu-id="9b830-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b830-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="9b830-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b830-134">Response</span></span>
<span data-ttu-id="9b830-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b830-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1425

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
      "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
      "displayName": "Display Name value",
      "description": "Description value",
      "permissions": [
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
      ],
      "rolePermissions": [
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
      ],
      "isBuiltInRoleDefinition": true,
      "isBuiltIn": true
    }
  ]
}
```





