---
title: Função getEffectivePermissions
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a1c2cb3ba99d89f2903fb417784cf08fdd1bd78f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898358"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="189b7-103">Função getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="189b7-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="189b7-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="189b7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="189b7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="189b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="189b7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="189b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="189b7-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="189b7-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="189b7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="189b7-108">Prerequisites</span></span>
<span data-ttu-id="189b7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="189b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="189b7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="189b7-111">Permission type</span></span>|<span data-ttu-id="189b7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="189b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="189b7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="189b7-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="189b7-114">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="189b7-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="189b7-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="189b7-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="189b7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="189b7-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="189b7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="189b7-117">Not supported.</span></span>|
|<span data-ttu-id="189b7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="189b7-118">Application</span></span>|<span data-ttu-id="189b7-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="189b7-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="189b7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="189b7-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="189b7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="189b7-121">Request headers</span></span>
|<span data-ttu-id="189b7-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="189b7-122">Header</span></span>|<span data-ttu-id="189b7-123">Valor</span><span class="sxs-lookup"><span data-stu-id="189b7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="189b7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="189b7-124">Authorization</span></span>|<span data-ttu-id="189b7-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="189b7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="189b7-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="189b7-126">Accept</span></span>|<span data-ttu-id="189b7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="189b7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="189b7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="189b7-128">Request body</span></span>
<span data-ttu-id="189b7-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="189b7-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="189b7-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="189b7-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="189b7-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="189b7-131">Property</span></span>|<span data-ttu-id="189b7-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="189b7-132">Type</span></span>|<span data-ttu-id="189b7-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="189b7-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="189b7-134">scope</span><span class="sxs-lookup"><span data-stu-id="189b7-134">scope</span></span>|<span data-ttu-id="189b7-135">String</span><span class="sxs-lookup"><span data-stu-id="189b7-135">String</span></span>|<span data-ttu-id="189b7-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="189b7-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="189b7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="189b7-137">Response</span></span>
<span data-ttu-id="189b7-138">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [rolePermission](../resources/intune-rbac-rolepermission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="189b7-138">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="189b7-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="189b7-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="189b7-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="189b7-140">Request</span></span>
<span data-ttu-id="189b7-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="189b7-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="189b7-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="189b7-142">Response</span></span>
<span data-ttu-id="189b7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="189b7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



