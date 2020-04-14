---
title: Função getEffectivePermissions
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ec8e3bf80ea0e9fb7077f3bac2d7bcf97c217d5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390165"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="2cfd4-103">Função getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="2cfd4-103">getEffectivePermissions function</span></span>

<span data-ttu-id="2cfd4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cfd4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2cfd4-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2cfd4-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2cfd4-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cfd4-108">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2cfd4-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2cfd4-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2cfd4-109">Prerequisites</span></span>
<span data-ttu-id="2cfd4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cfd4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cfd4-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2cfd4-112">Permission type</span></span>|<span data-ttu-id="2cfd4-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2cfd4-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cfd4-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2cfd4-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2cfd4-115">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="2cfd4-115">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="2cfd4-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cfd4-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="2cfd4-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2cfd4-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cfd4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-118">Not supported.</span></span>|
|<span data-ttu-id="2cfd4-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2cfd4-119">Application</span></span>||
| <span data-ttu-id="2cfd4-120">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="2cfd4-120">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="2cfd4-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cfd4-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cfd4-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2cfd4-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="2cfd4-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2cfd4-123">Request headers</span></span>
|<span data-ttu-id="2cfd4-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2cfd4-124">Header</span></span>|<span data-ttu-id="2cfd4-125">Valor</span><span class="sxs-lookup"><span data-stu-id="2cfd4-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cfd4-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="2cfd4-126">Authorization</span></span>|<span data-ttu-id="2cfd4-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cfd4-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2cfd4-128">Accept</span></span>|<span data-ttu-id="2cfd4-129">application/json</span><span class="sxs-lookup"><span data-stu-id="2cfd4-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cfd4-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2cfd4-130">Request body</span></span>
<span data-ttu-id="2cfd4-131">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="2cfd4-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="2cfd4-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2cfd4-133">Property</span></span>|<span data-ttu-id="2cfd4-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cfd4-134">Type</span></span>|<span data-ttu-id="2cfd4-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cfd4-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cfd4-136">scope</span><span class="sxs-lookup"><span data-stu-id="2cfd4-136">scope</span></span>|<span data-ttu-id="2cfd4-137">String</span><span class="sxs-lookup"><span data-stu-id="2cfd4-137">String</span></span>|<span data-ttu-id="2cfd4-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2cfd4-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2cfd4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cfd4-139">Response</span></span>
<span data-ttu-id="2cfd4-140">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [rolePermission](../resources/intune-rbac-rolepermission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-140">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cfd4-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2cfd4-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="2cfd4-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2cfd4-142">Request</span></span>
<span data-ttu-id="2cfd4-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="2cfd4-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cfd4-144">Response</span></span>
<span data-ttu-id="2cfd4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









