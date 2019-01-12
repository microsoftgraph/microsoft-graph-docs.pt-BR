---
title: Função getEffectivePermissions
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 978b615293e09d0f8b3f3c23fd17d3018fe17609
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973668"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="62478-103">Função getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="62478-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="62478-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="62478-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62478-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="62478-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62478-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="62478-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62478-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="62478-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="62478-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62478-108">Prerequisites</span></span>
<span data-ttu-id="62478-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62478-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62478-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62478-111">Permission type</span></span>|<span data-ttu-id="62478-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="62478-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62478-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62478-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="62478-114">&nbsp;&nbsp; **O controle de acesso baseado em função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="62478-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="62478-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="62478-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="62478-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62478-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62478-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62478-117">Not supported.</span></span>|
|<span data-ttu-id="62478-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62478-118">Application</span></span>|<span data-ttu-id="62478-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62478-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62478-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62478-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="62478-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62478-121">Request headers</span></span>
|<span data-ttu-id="62478-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62478-122">Header</span></span>|<span data-ttu-id="62478-123">Valor</span><span class="sxs-lookup"><span data-stu-id="62478-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62478-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="62478-124">Authorization</span></span>|<span data-ttu-id="62478-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62478-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62478-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62478-126">Accept</span></span>|<span data-ttu-id="62478-127">application/json</span><span class="sxs-lookup"><span data-stu-id="62478-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62478-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62478-128">Request body</span></span>
<span data-ttu-id="62478-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="62478-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="62478-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="62478-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="62478-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62478-131">Property</span></span>|<span data-ttu-id="62478-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="62478-132">Type</span></span>|<span data-ttu-id="62478-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="62478-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62478-134">scope</span><span class="sxs-lookup"><span data-stu-id="62478-134">scope</span></span>|<span data-ttu-id="62478-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62478-135">String</span></span>|<span data-ttu-id="62478-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="62478-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="62478-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="62478-137">Response</span></span>
<span data-ttu-id="62478-138">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [rolePermission](../resources/intune-rbac-rolepermission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62478-138">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62478-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62478-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="62478-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62478-140">Request</span></span>
<span data-ttu-id="62478-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62478-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="62478-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="62478-142">Response</span></span>
<span data-ttu-id="62478-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62478-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



