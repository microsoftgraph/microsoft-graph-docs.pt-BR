---
title: Função getEffectivePermissions
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: a4e188e9d8ec098f66274e9dbeecb852bb34914b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317854"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="7305a-103">Função getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="7305a-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="7305a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7305a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7305a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7305a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7305a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7305a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7305a-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7305a-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7305a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7305a-108">Prerequisites</span></span>
<span data-ttu-id="7305a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7305a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7305a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7305a-111">Permission type</span></span>|<span data-ttu-id="7305a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7305a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7305a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7305a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7305a-114">&nbsp;&nbsp; **O controle de acesso baseado em função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="7305a-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="7305a-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="7305a-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="7305a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7305a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7305a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7305a-117">Not supported.</span></span>|
|<span data-ttu-id="7305a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7305a-118">Application</span></span>|<span data-ttu-id="7305a-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7305a-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7305a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7305a-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="7305a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7305a-121">Request headers</span></span>
|<span data-ttu-id="7305a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7305a-122">Header</span></span>|<span data-ttu-id="7305a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7305a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7305a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7305a-124">Authorization</span></span>|<span data-ttu-id="7305a-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7305a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7305a-126">Accept</span><span class="sxs-lookup"><span data-stu-id="7305a-126">Accept</span></span>|<span data-ttu-id="7305a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7305a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7305a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7305a-128">Request body</span></span>
<span data-ttu-id="7305a-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="7305a-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7305a-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="7305a-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7305a-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7305a-131">Property</span></span>|<span data-ttu-id="7305a-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="7305a-132">Type</span></span>|<span data-ttu-id="7305a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="7305a-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7305a-134">scope</span><span class="sxs-lookup"><span data-stu-id="7305a-134">scope</span></span>|<span data-ttu-id="7305a-135">String</span><span class="sxs-lookup"><span data-stu-id="7305a-135">String</span></span>|<span data-ttu-id="7305a-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7305a-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7305a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7305a-137">Response</span></span>
<span data-ttu-id="7305a-138">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [rolePermission](../resources/intune-rbac-rolepermission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7305a-138">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7305a-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7305a-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="7305a-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7305a-140">Request</span></span>
<span data-ttu-id="7305a-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7305a-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="7305a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7305a-142">Response</span></span>
<span data-ttu-id="7305a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7305a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



