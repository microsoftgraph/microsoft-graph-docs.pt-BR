---
title: atribuir ação
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8c79825d3777bb5582f1715d1c0cc72103017ad7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425152"
---
# <a name="assign-action"></a><span data-ttu-id="b1326-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="b1326-103">assign action</span></span>

> <span data-ttu-id="b1326-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b1326-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b1326-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b1326-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1326-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b1326-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1326-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1326-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1326-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b1326-108">Prerequisites</span></span>
<span data-ttu-id="b1326-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b1326-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b1326-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1326-111">Permission type</span></span>|<span data-ttu-id="b1326-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b1326-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1326-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1326-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1326-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1326-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1326-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1326-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1326-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1326-116">Not supported.</span></span>|
|<span data-ttu-id="b1326-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1326-117">Application</span></span>|<span data-ttu-id="b1326-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1326-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1326-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1326-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="b1326-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1326-120">Request headers</span></span>
|<span data-ttu-id="b1326-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1326-121">Header</span></span>|<span data-ttu-id="b1326-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b1326-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1326-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1326-123">Authorization</span></span>|<span data-ttu-id="b1326-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1326-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1326-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b1326-125">Accept</span></span>|<span data-ttu-id="b1326-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1326-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1326-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1326-127">Request body</span></span>
<span data-ttu-id="b1326-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b1326-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b1326-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b1326-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b1326-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1326-130">Property</span></span>|<span data-ttu-id="b1326-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1326-131">Type</span></span>|<span data-ttu-id="b1326-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1326-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1326-133">assignments</span><span class="sxs-lookup"><span data-stu-id="b1326-133">assignments</span></span>|<span data-ttu-id="b1326-134">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b1326-134">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="b1326-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1326-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b1326-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1326-136">Response</span></span>
<span data-ttu-id="b1326-137">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1326-137">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1326-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1326-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1326-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1326-139">Request</span></span>
<span data-ttu-id="b1326-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1326-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign

Content-type: application/json
Content-length: 280

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
      "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b1326-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1326-141">Response</span></span>
<span data-ttu-id="b1326-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1326-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
      "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




