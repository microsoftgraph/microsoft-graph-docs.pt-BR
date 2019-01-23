---
title: função getManagementConditionsForPlatform
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2434d00c637112baa139ef92e4f77819ed8fd069
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420406"
---
# <a name="getmanagementconditionsforplatform-function"></a><span data-ttu-id="4bc39-103">função getManagementConditionsForPlatform</span><span class="sxs-lookup"><span data-stu-id="4bc39-103">getManagementConditionsForPlatform function</span></span>

> <span data-ttu-id="4bc39-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="4bc39-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4bc39-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4bc39-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4bc39-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="4bc39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bc39-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4bc39-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4bc39-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4bc39-108">Prerequisites</span></span>
<span data-ttu-id="4bc39-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4bc39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4bc39-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bc39-111">Permission type</span></span>|<span data-ttu-id="4bc39-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4bc39-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bc39-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bc39-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4bc39-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bc39-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4bc39-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bc39-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bc39-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bc39-116">Not supported.</span></span>|
|<span data-ttu-id="4bc39-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bc39-117">Application</span></span>|<span data-ttu-id="4bc39-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bc39-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bc39-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bc39-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/getManagementConditionsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/getManagementConditionsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="4bc39-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bc39-120">Request headers</span></span>
|<span data-ttu-id="4bc39-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4bc39-121">Header</span></span>|<span data-ttu-id="4bc39-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4bc39-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bc39-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bc39-123">Authorization</span></span>|<span data-ttu-id="4bc39-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bc39-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bc39-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4bc39-125">Accept</span></span>|<span data-ttu-id="4bc39-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4bc39-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bc39-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4bc39-127">Request body</span></span>
<span data-ttu-id="4bc39-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="4bc39-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="4bc39-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="4bc39-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4bc39-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4bc39-130">Property</span></span>|<span data-ttu-id="4bc39-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bc39-131">Type</span></span>|<span data-ttu-id="4bc39-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bc39-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bc39-133">platform</span><span class="sxs-lookup"><span data-stu-id="4bc39-133">platform</span></span>|[<span data-ttu-id="4bc39-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="4bc39-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="4bc39-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4bc39-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4bc39-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bc39-136">Response</span></span>
<span data-ttu-id="4bc39-137">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um conjunto de [managementCondition](../resources/intune-fencing-managementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bc39-137">If successful, this function returns a `200 OK` response code and a [managementCondition](../resources/intune-fencing-managementcondition.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bc39-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bc39-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="4bc39-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bc39-139">Request</span></span>
<span data-ttu-id="4bc39-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bc39-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/getManagementConditionsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="4bc39-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bc39-141">Response</span></span>
<span data-ttu-id="4bc39-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4bc39-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managementCondition",
      "id": "5cb49381-9381-5cb4-8193-b45c8193b45c",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```




