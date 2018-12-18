---
title: Excluir windows10SecureAssessmentConfiguration
description: Exclui windows10SecureAssessmentConfiguration.
author: tfitzmac
ms.openlocfilehash: 861848bc7525d47e6eb274a985a69bd2595cf0bf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325197"
---
# <a name="delete-windows10secureassessmentconfiguration"></a><span data-ttu-id="23195-103">Excluir windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="23195-103">Delete windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="23195-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="23195-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23195-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="23195-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23195-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="23195-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23195-107">Exclui [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23195-107">Deletes a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="23195-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="23195-108">Prerequisites</span></span>
<span data-ttu-id="23195-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23195-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23195-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23195-111">Permission type</span></span>|<span data-ttu-id="23195-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="23195-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23195-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23195-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23195-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23195-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23195-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23195-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23195-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23195-116">Not supported.</span></span>|
|<span data-ttu-id="23195-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23195-117">Application</span></span>|<span data-ttu-id="23195-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23195-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23195-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23195-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="23195-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23195-120">Request headers</span></span>
|<span data-ttu-id="23195-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="23195-121">Header</span></span>|<span data-ttu-id="23195-122">Valor</span><span class="sxs-lookup"><span data-stu-id="23195-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23195-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="23195-123">Authorization</span></span>|<span data-ttu-id="23195-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23195-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23195-125">Accept</span><span class="sxs-lookup"><span data-stu-id="23195-125">Accept</span></span>|<span data-ttu-id="23195-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23195-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23195-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23195-127">Request body</span></span>
<span data-ttu-id="23195-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23195-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23195-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="23195-129">Response</span></span>
<span data-ttu-id="23195-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="23195-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="23195-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23195-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="23195-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23195-132">Request</span></span>
<span data-ttu-id="23195-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23195-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="23195-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="23195-134">Response</span></span>
<span data-ttu-id="23195-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23195-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





