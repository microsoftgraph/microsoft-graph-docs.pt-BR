---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46b699aa1cb16edbbdd4da704f55625fc28a9adb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987996"
---
# <a name="assign-action"></a><span data-ttu-id="94af7-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="94af7-103">assign action</span></span>

> <span data-ttu-id="94af7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94af7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94af7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94af7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94af7-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="94af7-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94af7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="94af7-107">Prerequisites</span></span>
<span data-ttu-id="94af7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94af7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94af7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94af7-110">Permission type</span></span>|<span data-ttu-id="94af7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="94af7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94af7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94af7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94af7-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94af7-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="94af7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94af7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94af7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94af7-115">Not supported.</span></span>|
|<span data-ttu-id="94af7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94af7-116">Application</span></span>|<span data-ttu-id="94af7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94af7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94af7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94af7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="94af7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94af7-119">Request headers</span></span>
|<span data-ttu-id="94af7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94af7-120">Header</span></span>|<span data-ttu-id="94af7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="94af7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94af7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="94af7-122">Authorization</span></span>|<span data-ttu-id="94af7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94af7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94af7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="94af7-124">Accept</span></span>|<span data-ttu-id="94af7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="94af7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94af7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94af7-126">Request body</span></span>
<span data-ttu-id="94af7-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="94af7-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="94af7-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="94af7-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="94af7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94af7-129">Property</span></span>|<span data-ttu-id="94af7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="94af7-130">Type</span></span>|<span data-ttu-id="94af7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="94af7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94af7-132">enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="94af7-132">enrollmentConfigurationAssignments</span></span>|<span data-ttu-id="94af7-133">Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="94af7-133">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="94af7-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="94af7-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="94af7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="94af7-135">Response</span></span>
<span data-ttu-id="94af7-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="94af7-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="94af7-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94af7-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="94af7-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94af7-138">Request</span></span>
<span data-ttu-id="94af7-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94af7-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="94af7-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="94af7-140">Response</span></span>
<span data-ttu-id="94af7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94af7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





