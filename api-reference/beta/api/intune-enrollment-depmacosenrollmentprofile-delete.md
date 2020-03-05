---
title: Excluir depMacOSEnrollmentProfile
description: Exclui depMacOSEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 041f4fb96419e00bce7566bf6fdaf9567b362d54
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467127"
---
# <a name="delete-depmacosenrollmentprofile"></a><span data-ttu-id="4cfcf-103">Excluir depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="4cfcf-103">Delete depMacOSEnrollmentProfile</span></span>

<span data-ttu-id="4cfcf-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4cfcf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4cfcf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4cfcf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cfcf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4cfcf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cfcf-107">Exclui [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="4cfcf-107">Deletes a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4cfcf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4cfcf-108">Prerequisites</span></span>
<span data-ttu-id="4cfcf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cfcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cfcf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4cfcf-111">Permission type</span></span>|<span data-ttu-id="4cfcf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4cfcf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cfcf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4cfcf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4cfcf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cfcf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4cfcf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4cfcf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cfcf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4cfcf-116">Not supported.</span></span>|
|<span data-ttu-id="4cfcf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4cfcf-117">Application</span></span>|<span data-ttu-id="4cfcf-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cfcf-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cfcf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4cfcf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="4cfcf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4cfcf-120">Request headers</span></span>
|<span data-ttu-id="4cfcf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4cfcf-121">Header</span></span>|<span data-ttu-id="4cfcf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4cfcf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cfcf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4cfcf-123">Authorization</span></span>|<span data-ttu-id="4cfcf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4cfcf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cfcf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4cfcf-125">Accept</span></span>|<span data-ttu-id="4cfcf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4cfcf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cfcf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4cfcf-127">Request body</span></span>
<span data-ttu-id="4cfcf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4cfcf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cfcf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cfcf-129">Response</span></span>
<span data-ttu-id="4cfcf-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4cfcf-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4cfcf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4cfcf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4cfcf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4cfcf-132">Request</span></span>
<span data-ttu-id="4cfcf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4cfcf-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="4cfcf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cfcf-134">Response</span></span>
<span data-ttu-id="4cfcf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4cfcf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





