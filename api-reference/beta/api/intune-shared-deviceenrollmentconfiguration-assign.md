---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 05372ef09bcff5dd6d1f671f03425c0f7ea86c31
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702940"
---
# <a name="assign-action"></a><span data-ttu-id="88d87-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="88d87-103">assign action</span></span>

<span data-ttu-id="88d87-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88d87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88d87-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88d87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88d87-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88d87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88d87-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="88d87-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88d87-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88d87-108">Prerequisites</span></span>
<span data-ttu-id="88d87-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88d87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88d87-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88d87-111">Permission type</span></span>|<span data-ttu-id="88d87-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="88d87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88d87-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88d87-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="88d87-114">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="88d87-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="88d87-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88d87-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="88d87-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88d87-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88d87-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88d87-117">Not supported.</span></span>|
|<span data-ttu-id="88d87-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88d87-118">Application</span></span>||
| <span data-ttu-id="88d87-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="88d87-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="88d87-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88d87-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88d87-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88d87-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="88d87-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88d87-122">Request headers</span></span>
|<span data-ttu-id="88d87-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88d87-123">Header</span></span>|<span data-ttu-id="88d87-124">Valor</span><span class="sxs-lookup"><span data-stu-id="88d87-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88d87-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="88d87-125">Authorization</span></span>|<span data-ttu-id="88d87-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88d87-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88d87-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="88d87-127">Accept</span></span>|<span data-ttu-id="88d87-128">application/json</span><span class="sxs-lookup"><span data-stu-id="88d87-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88d87-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88d87-129">Request body</span></span>
<span data-ttu-id="88d87-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="88d87-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="88d87-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="88d87-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="88d87-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88d87-132">Property</span></span>|<span data-ttu-id="88d87-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="88d87-133">Type</span></span>|<span data-ttu-id="88d87-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="88d87-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88d87-135">enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="88d87-135">enrollmentConfigurationAssignments</span></span>|<span data-ttu-id="88d87-136">Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="88d87-136">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="88d87-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="88d87-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="88d87-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="88d87-138">Response</span></span>
<span data-ttu-id="88d87-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="88d87-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="88d87-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88d87-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="88d87-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88d87-141">Request</span></span>
<span data-ttu-id="88d87-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88d87-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign

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

### <a name="response"></a><span data-ttu-id="88d87-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="88d87-143">Response</span></span>
<span data-ttu-id="88d87-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88d87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








