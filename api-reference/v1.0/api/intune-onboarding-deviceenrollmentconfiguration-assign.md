---
title: atribuir ação
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a67fecb2916b0394a9562d29692233ce9188f59e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961018"
---
# <a name="assign-action"></a><span data-ttu-id="fab34-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="fab34-103">assign action</span></span>

> <span data-ttu-id="fab34-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fab34-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fab34-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fab34-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fab34-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fab34-106">Prerequisites</span></span>
<span data-ttu-id="fab34-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fab34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fab34-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fab34-109">Permission type</span></span>|<span data-ttu-id="fab34-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fab34-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fab34-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fab34-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fab34-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fab34-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fab34-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fab34-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fab34-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fab34-114">Not supported.</span></span>|
|<span data-ttu-id="fab34-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fab34-115">Application</span></span>|<span data-ttu-id="fab34-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fab34-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fab34-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fab34-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="fab34-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fab34-118">Request headers</span></span>
|<span data-ttu-id="fab34-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fab34-119">Header</span></span>|<span data-ttu-id="fab34-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fab34-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fab34-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fab34-121">Authorization</span></span>|<span data-ttu-id="fab34-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fab34-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fab34-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fab34-123">Accept</span></span>|<span data-ttu-id="fab34-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fab34-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fab34-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fab34-125">Request body</span></span>
<span data-ttu-id="fab34-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="fab34-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fab34-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="fab34-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fab34-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fab34-128">Property</span></span>|<span data-ttu-id="fab34-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="fab34-129">Type</span></span>|<span data-ttu-id="fab34-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="fab34-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fab34-131">enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="fab34-131">enrollmentConfigurationAssignments</span></span>|<span data-ttu-id="fab34-132">Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="fab34-132">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="fab34-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fab34-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fab34-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fab34-134">Response</span></span>
<span data-ttu-id="fab34-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fab34-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fab34-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fab34-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="fab34-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fab34-137">Request</span></span>
<span data-ttu-id="fab34-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fab34-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign

Content-type: application/json
Content-length: 304

{
  "enrollmentConfigurationAssignments": [
    {
      "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
      "id": "705b021c-021c-705b-1c02-5b701c025b70",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="fab34-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fab34-139">Response</span></span>
<span data-ttu-id="fab34-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fab34-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



