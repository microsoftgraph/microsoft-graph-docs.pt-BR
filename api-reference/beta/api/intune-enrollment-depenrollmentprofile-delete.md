---
title: Excluir depEnrollmentProfile
description: Exclui depEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ced4abf5df00a4d0367b5a13cf7e742addcf083
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090320"
---
# <a name="delete-depenrollmentprofile"></a><span data-ttu-id="c631d-103">Excluir depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c631d-103">Delete depEnrollmentProfile</span></span>

<span data-ttu-id="c631d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c631d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c631d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c631d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c631d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c631d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c631d-107">Exclui [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="c631d-107">Deletes a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c631d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c631d-108">Prerequisites</span></span>
<span data-ttu-id="c631d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c631d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c631d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c631d-111">Permission type</span></span>|<span data-ttu-id="c631d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c631d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c631d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c631d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c631d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c631d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c631d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c631d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c631d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c631d-116">Not supported.</span></span>|
|<span data-ttu-id="c631d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c631d-117">Application</span></span>|<span data-ttu-id="c631d-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c631d-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c631d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c631d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="c631d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c631d-120">Request headers</span></span>
|<span data-ttu-id="c631d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c631d-121">Header</span></span>|<span data-ttu-id="c631d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c631d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c631d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c631d-123">Authorization</span></span>|<span data-ttu-id="c631d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c631d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c631d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c631d-125">Accept</span></span>|<span data-ttu-id="c631d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c631d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c631d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c631d-127">Request body</span></span>
<span data-ttu-id="c631d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c631d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c631d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c631d-129">Response</span></span>
<span data-ttu-id="c631d-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c631d-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c631d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c631d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c631d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c631d-132">Request</span></span>
<span data-ttu-id="c631d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c631d-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="c631d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c631d-134">Response</span></span>
<span data-ttu-id="c631d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c631d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






