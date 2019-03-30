---
title: Excluir depMacOSEnrollmentProfile
description: Exclui depMacOSEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 053985ab71c863c07e12aefcaa68819f64caabe7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989152"
---
# <a name="delete-depmacosenrollmentprofile"></a><span data-ttu-id="15090-103">Excluir depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="15090-103">Delete depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="15090-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="15090-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15090-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15090-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15090-106">Exclui [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="15090-106">Deletes a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15090-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15090-107">Prerequisites</span></span>
<span data-ttu-id="15090-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15090-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15090-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15090-110">Permission type</span></span>|<span data-ttu-id="15090-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15090-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15090-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15090-112">Delegated (work or school account)</span></span>|<span data-ttu-id="15090-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15090-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="15090-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15090-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15090-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15090-115">Not supported.</span></span>|
|<span data-ttu-id="15090-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15090-116">Application</span></span>|<span data-ttu-id="15090-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15090-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15090-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15090-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="15090-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15090-119">Request headers</span></span>
|<span data-ttu-id="15090-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15090-120">Header</span></span>|<span data-ttu-id="15090-121">Valor</span><span class="sxs-lookup"><span data-stu-id="15090-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15090-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="15090-122">Authorization</span></span>|<span data-ttu-id="15090-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15090-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15090-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15090-124">Accept</span></span>|<span data-ttu-id="15090-125">application/json</span><span class="sxs-lookup"><span data-stu-id="15090-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15090-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15090-126">Request body</span></span>
<span data-ttu-id="15090-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15090-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15090-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="15090-128">Response</span></span>
<span data-ttu-id="15090-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="15090-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="15090-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15090-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="15090-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15090-131">Request</span></span>
<span data-ttu-id="15090-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15090-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="15090-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="15090-133">Response</span></span>
<span data-ttu-id="15090-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15090-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




