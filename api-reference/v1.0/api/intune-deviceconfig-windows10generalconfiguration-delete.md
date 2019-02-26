---
title: Excluir windows10GeneralConfiguration
description: Exclui windows10GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 670c4ee3703728c01c4d2491912bad97c503bcea
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260589"
---
# <a name="delete-windows10generalconfiguration"></a><span data-ttu-id="880f9-103">Excluir windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="880f9-103">Delete windows10GeneralConfiguration</span></span>

> <span data-ttu-id="880f9-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="880f9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="880f9-105">Exclui [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="880f9-105">Deletes a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="880f9-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="880f9-106">Prerequisites</span></span>
<span data-ttu-id="880f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="880f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="880f9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="880f9-109">Permission type</span></span>|<span data-ttu-id="880f9-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="880f9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="880f9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="880f9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="880f9-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="880f9-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="880f9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="880f9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="880f9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="880f9-114">Not supported.</span></span>|
|<span data-ttu-id="880f9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="880f9-115">Application</span></span>|<span data-ttu-id="880f9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="880f9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="880f9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="880f9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="880f9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="880f9-118">Request headers</span></span>
|<span data-ttu-id="880f9-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="880f9-119">Header</span></span>|<span data-ttu-id="880f9-120">Valor</span><span class="sxs-lookup"><span data-stu-id="880f9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="880f9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="880f9-121">Authorization</span></span>|<span data-ttu-id="880f9-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="880f9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="880f9-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="880f9-123">Accept</span></span>|<span data-ttu-id="880f9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="880f9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="880f9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="880f9-125">Request body</span></span>
<span data-ttu-id="880f9-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="880f9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="880f9-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="880f9-127">Response</span></span>
<span data-ttu-id="880f9-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="880f9-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="880f9-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="880f9-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="880f9-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="880f9-130">Request</span></span>
<span data-ttu-id="880f9-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="880f9-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="880f9-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="880f9-132">Response</span></span>
<span data-ttu-id="880f9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="880f9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



