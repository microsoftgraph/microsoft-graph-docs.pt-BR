---
title: Atualizar reportRoot
description: Atualizar as propriedades de um objeto reportRoot.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: da9ff796f3c2eabf01bff459850e259fea0c81ba
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195801"
---
# <a name="update-reportroot"></a><span data-ttu-id="4e75d-103">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="4e75d-103">Update reportRoot</span></span>

> <span data-ttu-id="4e75d-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4e75d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4e75d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4e75d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e75d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e75d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e75d-107">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="4e75d-107">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e75d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4e75d-108">Prerequisites</span></span>
<span data-ttu-id="4e75d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e75d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e75d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e75d-111">Permission type</span></span>|<span data-ttu-id="4e75d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4e75d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e75d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e75d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4e75d-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="4e75d-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4e75d-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e75d-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="4e75d-116">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="4e75d-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="4e75d-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e75d-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4e75d-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e75d-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e75d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e75d-119">Not supported.</span></span>|
|<span data-ttu-id="4e75d-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e75d-120">Application</span></span>||
| <span data-ttu-id="4e75d-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="4e75d-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4e75d-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e75d-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="4e75d-123">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="4e75d-123">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="4e75d-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e75d-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e75d-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e75d-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="4e75d-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e75d-126">Request headers</span></span>
|<span data-ttu-id="4e75d-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e75d-127">Header</span></span>|<span data-ttu-id="4e75d-128">Valor</span><span class="sxs-lookup"><span data-stu-id="4e75d-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e75d-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e75d-129">Authorization</span></span>|<span data-ttu-id="4e75d-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e75d-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e75d-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4e75d-131">Accept</span></span>|<span data-ttu-id="4e75d-132">application/json</span><span class="sxs-lookup"><span data-stu-id="4e75d-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e75d-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e75d-133">Request body</span></span>
<span data-ttu-id="4e75d-134">No corpo da solicitação, forneça uma representação JSON do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="4e75d-134">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="4e75d-135">A tabela a seguir mostra as propriedades que são necessárias ao criar [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="4e75d-135">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="4e75d-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e75d-136">Property</span></span>|<span data-ttu-id="4e75d-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e75d-137">Type</span></span>|<span data-ttu-id="4e75d-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e75d-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e75d-139">id</span><span class="sxs-lookup"><span data-stu-id="4e75d-139">id</span></span>|<span data-ttu-id="4e75d-140">String</span><span class="sxs-lookup"><span data-stu-id="4e75d-140">String</span></span>|<span data-ttu-id="4e75d-141">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="4e75d-141">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="4e75d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e75d-142">Response</span></span>
<span data-ttu-id="4e75d-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e75d-143">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e75d-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e75d-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="4e75d-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e75d-145">Request</span></span>
<span data-ttu-id="4e75d-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e75d-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="4e75d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e75d-147">Response</span></span>
<span data-ttu-id="4e75d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e75d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```







