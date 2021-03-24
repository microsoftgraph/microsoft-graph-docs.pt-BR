---
title: Excluir depEnrollmentProfile
description: Exclui um depEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f95c8dfb043f626969fa2af94ce4953782cbca4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135793"
---
# <a name="delete-depenrollmentprofile"></a><span data-ttu-id="76e34-103">Excluir depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="76e34-103">Delete depEnrollmentProfile</span></span>

<span data-ttu-id="76e34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76e34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76e34-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="76e34-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76e34-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76e34-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76e34-107">Exclui um [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="76e34-107">Deletes a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76e34-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="76e34-108">Prerequisites</span></span>
<span data-ttu-id="76e34-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76e34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76e34-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76e34-111">Permission type</span></span>|<span data-ttu-id="76e34-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76e34-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76e34-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76e34-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76e34-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76e34-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="76e34-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76e34-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76e34-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76e34-116">Not supported.</span></span>|
|<span data-ttu-id="76e34-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76e34-117">Application</span></span>|<span data-ttu-id="76e34-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76e34-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76e34-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76e34-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="76e34-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76e34-120">Request headers</span></span>
|<span data-ttu-id="76e34-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76e34-121">Header</span></span>|<span data-ttu-id="76e34-122">Valor</span><span class="sxs-lookup"><span data-stu-id="76e34-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76e34-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="76e34-123">Authorization</span></span>|<span data-ttu-id="76e34-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76e34-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76e34-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="76e34-125">Accept</span></span>|<span data-ttu-id="76e34-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76e34-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76e34-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76e34-127">Request body</span></span>
<span data-ttu-id="76e34-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="76e34-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76e34-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="76e34-129">Response</span></span>
<span data-ttu-id="76e34-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="76e34-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="76e34-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76e34-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="76e34-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76e34-132">Request</span></span>
<span data-ttu-id="76e34-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76e34-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="76e34-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="76e34-134">Response</span></span>
<span data-ttu-id="76e34-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76e34-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




