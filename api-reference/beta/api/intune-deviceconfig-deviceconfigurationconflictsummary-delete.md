---
title: Excluir deviceConfigurationConflictSummary
description: Exclui um deviceConfigurationConflictSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 25491d368cb63daf9968415ee0eb15120e11a0a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882366"
---
# <a name="delete-deviceconfigurationconflictsummary"></a><span data-ttu-id="dab2e-103">Excluir deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="dab2e-103">Delete deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="dab2e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dab2e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dab2e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dab2e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dab2e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dab2e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dab2e-107">Exclui um [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span><span class="sxs-lookup"><span data-stu-id="dab2e-107">Deletes a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dab2e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dab2e-108">Prerequisites</span></span>
<span data-ttu-id="dab2e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dab2e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dab2e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dab2e-111">Permission type</span></span>|<span data-ttu-id="dab2e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dab2e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dab2e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dab2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dab2e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dab2e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dab2e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dab2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dab2e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dab2e-116">Not supported.</span></span>|
|<span data-ttu-id="dab2e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dab2e-117">Application</span></span>|<span data-ttu-id="dab2e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dab2e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dab2e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dab2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="dab2e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dab2e-120">Request headers</span></span>
|<span data-ttu-id="dab2e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dab2e-121">Header</span></span>|<span data-ttu-id="dab2e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dab2e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dab2e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dab2e-123">Authorization</span></span>|<span data-ttu-id="dab2e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dab2e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dab2e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dab2e-125">Accept</span></span>|<span data-ttu-id="dab2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dab2e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dab2e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dab2e-127">Request body</span></span>
<span data-ttu-id="dab2e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dab2e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dab2e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dab2e-129">Response</span></span>
<span data-ttu-id="dab2e-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dab2e-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dab2e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dab2e-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="dab2e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dab2e-132">Request</span></span>
<span data-ttu-id="dab2e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dab2e-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

### <a name="response"></a><span data-ttu-id="dab2e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dab2e-134">Response</span></span>
<span data-ttu-id="dab2e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dab2e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





