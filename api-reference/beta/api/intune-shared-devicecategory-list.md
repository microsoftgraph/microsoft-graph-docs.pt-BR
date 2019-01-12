---
title: Listar deviceCategories
description: Lista propriedades e relações dos objetos deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f54865cd8156b1661f2312cf0335b99f08dd90be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950288"
---
# <a name="list-devicecategories"></a><span data-ttu-id="af325-103">Listar deviceCategories</span><span class="sxs-lookup"><span data-stu-id="af325-103">List deviceCategories</span></span>

> <span data-ttu-id="af325-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="af325-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af325-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="af325-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af325-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="af325-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af325-107">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="af325-107">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af325-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="af325-108">Prerequisites</span></span>
<span data-ttu-id="af325-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af325-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af325-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af325-111">Permission type</span></span>|<span data-ttu-id="af325-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="af325-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af325-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af325-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="af325-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="af325-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="af325-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="af325-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="af325-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af325-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af325-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af325-117">Not supported.</span></span>|
|<span data-ttu-id="af325-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af325-118">Application</span></span>|<span data-ttu-id="af325-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af325-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af325-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af325-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="af325-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af325-121">Request headers</span></span>

|<span data-ttu-id="af325-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af325-122">Header</span></span>|<span data-ttu-id="af325-123">Valor</span><span class="sxs-lookup"><span data-stu-id="af325-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af325-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="af325-124">Authorization</span></span>|<span data-ttu-id="af325-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af325-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af325-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="af325-126">Accept</span></span>|<span data-ttu-id="af325-127">application/json</span><span class="sxs-lookup"><span data-stu-id="af325-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af325-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af325-128">Request body</span></span>

<span data-ttu-id="af325-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af325-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af325-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="af325-130">Response</span></span>

<span data-ttu-id="af325-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af325-131">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af325-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af325-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="af325-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af325-133">Request</span></span>

<span data-ttu-id="af325-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af325-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="af325-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="af325-135">Response</span></span>

<span data-ttu-id="af325-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af325-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCategory",
      "id": "f881b841-b841-f881-41b8-81f841b881f8",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```



