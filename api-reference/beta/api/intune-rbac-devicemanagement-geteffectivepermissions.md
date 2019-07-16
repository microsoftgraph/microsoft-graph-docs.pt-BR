---
title: Função getEffectivePermissions
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 830fc92e6abc94c2616633a68b3a5580f29b09eb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725834"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="b087e-103">Função getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="b087e-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="b087e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b087e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b087e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b087e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b087e-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b087e-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b087e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b087e-107">Prerequisites</span></span>
<span data-ttu-id="b087e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b087e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b087e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b087e-110">Permission type</span></span>|<span data-ttu-id="b087e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b087e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b087e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b087e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b087e-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="b087e-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="b087e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b087e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b087e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b087e-115">Not supported.</span></span>|
|<span data-ttu-id="b087e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b087e-116">Application</span></span>|<span data-ttu-id="b087e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b087e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b087e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b087e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="b087e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b087e-119">Request headers</span></span>
|<span data-ttu-id="b087e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b087e-120">Header</span></span>|<span data-ttu-id="b087e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b087e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b087e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b087e-122">Authorization</span></span>|<span data-ttu-id="b087e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b087e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b087e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b087e-124">Accept</span></span>|<span data-ttu-id="b087e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b087e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b087e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b087e-126">Request body</span></span>
<span data-ttu-id="b087e-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="b087e-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b087e-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="b087e-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b087e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b087e-129">Property</span></span>|<span data-ttu-id="b087e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b087e-130">Type</span></span>|<span data-ttu-id="b087e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b087e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b087e-132">scope</span><span class="sxs-lookup"><span data-stu-id="b087e-132">scope</span></span>|<span data-ttu-id="b087e-133">String</span><span class="sxs-lookup"><span data-stu-id="b087e-133">String</span></span>|<span data-ttu-id="b087e-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b087e-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b087e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b087e-135">Response</span></span>
<span data-ttu-id="b087e-136">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [rolePermission](../resources/intune-rbac-rolepermission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b087e-136">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b087e-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b087e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="b087e-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b087e-138">Request</span></span>
<span data-ttu-id="b087e-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b087e-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b087e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b087e-140">Response</span></span>
<span data-ttu-id="b087e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b087e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





