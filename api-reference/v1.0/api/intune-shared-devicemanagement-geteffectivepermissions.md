---
title: Função getEffectivePermissions
description: Recupera permissões efetivas de usuário autenticado no momento
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f40412a8d95fd6bde17843b0c13e81f00459dd12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980073"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="0c728-103">Função getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="0c728-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="0c728-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0c728-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c728-105">Recupera permissões efetivas de usuário autenticado no momento</span><span class="sxs-lookup"><span data-stu-id="0c728-105">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c728-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c728-106">Prerequisites</span></span>
<span data-ttu-id="0c728-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c728-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c728-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c728-109">Permission type</span></span>|<span data-ttu-id="0c728-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0c728-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c728-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c728-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0c728-112">&nbsp;&nbsp; Controle de acesso baseado em função</span><span class="sxs-lookup"><span data-stu-id="0c728-112">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="0c728-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c728-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="0c728-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c728-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c728-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c728-115">Not supported.</span></span>|
|<span data-ttu-id="0c728-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c728-116">Application</span></span>|<span data-ttu-id="0c728-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c728-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c728-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c728-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="0c728-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c728-119">Request headers</span></span>
|<span data-ttu-id="0c728-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c728-120">Header</span></span>|<span data-ttu-id="0c728-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0c728-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c728-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c728-122">Authorization</span></span>|<span data-ttu-id="0c728-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c728-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c728-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c728-124">Accept</span></span>|<span data-ttu-id="0c728-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c728-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c728-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c728-126">Request body</span></span>
<span data-ttu-id="0c728-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="0c728-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="0c728-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="0c728-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="0c728-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c728-129">Property</span></span>|<span data-ttu-id="0c728-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c728-130">Type</span></span>|<span data-ttu-id="0c728-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c728-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c728-132">scope</span><span class="sxs-lookup"><span data-stu-id="0c728-132">scope</span></span>|<span data-ttu-id="0c728-133">String</span><span class="sxs-lookup"><span data-stu-id="0c728-133">String</span></span>|<span data-ttu-id="0c728-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0c728-134">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="0c728-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c728-135">Response</span></span>
<span data-ttu-id="0c728-136">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [rolePermission](../resources/intune-rbac-rolepermission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c728-136">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c728-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c728-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="0c728-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c728-138">Request</span></span>
<span data-ttu-id="0c728-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c728-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="0c728-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c728-140">Response</span></span>
<span data-ttu-id="0c728-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c728-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



