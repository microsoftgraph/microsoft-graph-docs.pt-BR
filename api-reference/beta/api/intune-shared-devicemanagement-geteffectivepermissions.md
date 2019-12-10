---
title: Função getEffectivePermissions
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3577e53935d1312e9d6963c9e36433ace8aef336
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939988"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="1fed9-103">Função getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="1fed9-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="1fed9-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1fed9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1fed9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1fed9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1fed9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1fed9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fed9-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1fed9-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1fed9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1fed9-108">Prerequisites</span></span>
<span data-ttu-id="1fed9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fed9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fed9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fed9-111">Permission type</span></span>|<span data-ttu-id="1fed9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1fed9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fed9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fed9-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1fed9-114">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="1fed9-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="1fed9-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fed9-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="1fed9-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fed9-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fed9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fed9-117">Not supported.</span></span>|
|<span data-ttu-id="1fed9-118">Application</span><span class="sxs-lookup"><span data-stu-id="1fed9-118">Application</span></span>||
| <span data-ttu-id="1fed9-119">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="1fed9-119">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="1fed9-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fed9-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fed9-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fed9-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="1fed9-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fed9-122">Request headers</span></span>
|<span data-ttu-id="1fed9-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1fed9-123">Header</span></span>|<span data-ttu-id="1fed9-124">Valor</span><span class="sxs-lookup"><span data-stu-id="1fed9-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fed9-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fed9-125">Authorization</span></span>|<span data-ttu-id="1fed9-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fed9-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fed9-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1fed9-127">Accept</span></span>|<span data-ttu-id="1fed9-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1fed9-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fed9-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fed9-129">Request body</span></span>
<span data-ttu-id="1fed9-130">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="1fed9-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="1fed9-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="1fed9-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="1fed9-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fed9-132">Property</span></span>|<span data-ttu-id="1fed9-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fed9-133">Type</span></span>|<span data-ttu-id="1fed9-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fed9-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fed9-135">scope</span><span class="sxs-lookup"><span data-stu-id="1fed9-135">scope</span></span>|<span data-ttu-id="1fed9-136">String</span><span class="sxs-lookup"><span data-stu-id="1fed9-136">String</span></span>|<span data-ttu-id="1fed9-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1fed9-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1fed9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fed9-138">Response</span></span>
<span data-ttu-id="1fed9-139">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [rolePermission](../resources/intune-rbac-rolepermission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fed9-139">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fed9-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1fed9-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="1fed9-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fed9-141">Request</span></span>
<span data-ttu-id="1fed9-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fed9-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="1fed9-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fed9-143">Response</span></span>
<span data-ttu-id="1fed9-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1fed9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











