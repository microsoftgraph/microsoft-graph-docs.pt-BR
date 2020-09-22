---
title: Atualizar reportRoot
description: Atualizar as propriedades de um objeto reportRoot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9c04831cf419d85a3d055462f4f42cf275c0afa2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053710"
---
# <a name="update-reportroot"></a><span data-ttu-id="fac0c-103">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="fac0c-103">Update reportRoot</span></span>

<span data-ttu-id="fac0c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fac0c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fac0c-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fac0c-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fac0c-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fac0c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fac0c-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fac0c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fac0c-108">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="fac0c-108">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fac0c-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fac0c-109">Prerequisites</span></span>
<span data-ttu-id="fac0c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fac0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fac0c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fac0c-112">Permission type</span></span>|<span data-ttu-id="fac0c-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fac0c-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fac0c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fac0c-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fac0c-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="fac0c-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="fac0c-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fac0c-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="fac0c-117">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="fac0c-117">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="fac0c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fac0c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fac0c-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fac0c-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fac0c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fac0c-120">Not supported.</span></span>|
|<span data-ttu-id="fac0c-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fac0c-121">Application</span></span>||
| <span data-ttu-id="fac0c-122">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="fac0c-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="fac0c-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fac0c-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="fac0c-124">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="fac0c-124">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="fac0c-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fac0c-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fac0c-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fac0c-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="fac0c-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fac0c-127">Request headers</span></span>
|<span data-ttu-id="fac0c-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fac0c-128">Header</span></span>|<span data-ttu-id="fac0c-129">Valor</span><span class="sxs-lookup"><span data-stu-id="fac0c-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fac0c-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="fac0c-130">Authorization</span></span>|<span data-ttu-id="fac0c-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fac0c-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fac0c-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fac0c-132">Accept</span></span>|<span data-ttu-id="fac0c-133">application/json</span><span class="sxs-lookup"><span data-stu-id="fac0c-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fac0c-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fac0c-134">Request body</span></span>
<span data-ttu-id="fac0c-135">No corpo da solicitação, forneça uma representação JSON do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="fac0c-135">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="fac0c-136">A tabela a seguir mostra as propriedades que são necessárias ao criar [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="fac0c-136">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="fac0c-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fac0c-137">Property</span></span>|<span data-ttu-id="fac0c-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="fac0c-138">Type</span></span>|<span data-ttu-id="fac0c-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="fac0c-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fac0c-140">id</span><span class="sxs-lookup"><span data-stu-id="fac0c-140">id</span></span>|<span data-ttu-id="fac0c-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fac0c-141">String</span></span>|<span data-ttu-id="fac0c-142">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="fac0c-142">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="fac0c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="fac0c-143">Response</span></span>
<span data-ttu-id="fac0c-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fac0c-144">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fac0c-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fac0c-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="fac0c-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fac0c-146">Request</span></span>
<span data-ttu-id="fac0c-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fac0c-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="fac0c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="fac0c-148">Response</span></span>
<span data-ttu-id="fac0c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fac0c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```












