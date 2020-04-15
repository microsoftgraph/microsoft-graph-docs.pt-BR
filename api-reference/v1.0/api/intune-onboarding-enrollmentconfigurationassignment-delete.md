---
title: Excluir enrollmentConfigurationAssignment
description: Exclui enrollmentConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 375fd24eb693a632fbb9fea2d88471a546390adf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442444"
---
# <a name="delete-enrollmentconfigurationassignment"></a><span data-ttu-id="c5776-103">Excluir enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c5776-103">Delete enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="c5776-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5776-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5776-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5776-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5776-106">Exclui [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c5776-106">Deletes a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5776-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c5776-107">Prerequisites</span></span>
<span data-ttu-id="c5776-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5776-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5776-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5776-110">Permission type</span></span>|<span data-ttu-id="c5776-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c5776-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5776-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5776-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5776-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5776-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c5776-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5776-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5776-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5776-115">Not supported.</span></span>|
|<span data-ttu-id="c5776-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5776-116">Application</span></span>|<span data-ttu-id="c5776-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5776-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5776-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5776-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c5776-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5776-119">Request headers</span></span>
|<span data-ttu-id="c5776-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5776-120">Header</span></span>|<span data-ttu-id="c5776-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c5776-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5776-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5776-122">Authorization</span></span>|<span data-ttu-id="c5776-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5776-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5776-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c5776-124">Accept</span></span>|<span data-ttu-id="c5776-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5776-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5776-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5776-126">Request body</span></span>
<span data-ttu-id="c5776-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5776-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5776-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5776-128">Response</span></span>
<span data-ttu-id="c5776-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c5776-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c5776-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5776-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5776-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5776-131">Request</span></span>
<span data-ttu-id="c5776-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5776-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="c5776-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5776-133">Response</span></span>
<span data-ttu-id="c5776-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5776-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






