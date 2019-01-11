---
title: Criar cartToClassAssociation
description: Crie um novo objeto de cartToClassAssociation.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6e3582f3f38258db75236b6cc877a64471da4b85
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822705"
---
# <a name="create-carttoclassassociation"></a><span data-ttu-id="2620f-103">Criar cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="2620f-103">Create cartToClassAssociation</span></span>

> <span data-ttu-id="2620f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2620f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2620f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2620f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2620f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2620f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2620f-107">Crie um novo objeto de [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="2620f-107">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2620f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2620f-108">Prerequisites</span></span>
<span data-ttu-id="2620f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2620f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2620f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2620f-111">Permission type</span></span>|<span data-ttu-id="2620f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2620f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2620f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2620f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2620f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2620f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2620f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2620f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2620f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2620f-116">Not supported.</span></span>|
|<span data-ttu-id="2620f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2620f-117">Application</span></span>|<span data-ttu-id="2620f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2620f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2620f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2620f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="2620f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2620f-120">Request headers</span></span>
|<span data-ttu-id="2620f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2620f-121">Header</span></span>|<span data-ttu-id="2620f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2620f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2620f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2620f-123">Authorization</span></span>|<span data-ttu-id="2620f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2620f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2620f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2620f-125">Accept</span></span>|<span data-ttu-id="2620f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2620f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2620f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2620f-127">Request body</span></span>
<span data-ttu-id="2620f-128">No corpo da solicitação, fornece uma representação JSON para o objeto cartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="2620f-128">In the request body, supply a JSON representation for the cartToClassAssociation object.</span></span>

<span data-ttu-id="2620f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o cartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="2620f-129">The following table shows the properties that are required when you create the cartToClassAssociation.</span></span>

|<span data-ttu-id="2620f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2620f-130">Property</span></span>|<span data-ttu-id="2620f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2620f-131">Type</span></span>|<span data-ttu-id="2620f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2620f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2620f-133">id</span><span class="sxs-lookup"><span data-stu-id="2620f-133">id</span></span>|<span data-ttu-id="2620f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2620f-134">String</span></span>|<span data-ttu-id="2620f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2620f-135">Key of the entity.</span></span>|
|<span data-ttu-id="2620f-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2620f-136">createdDateTime</span></span>|<span data-ttu-id="2620f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2620f-137">DateTimeOffset</span></span>|<span data-ttu-id="2620f-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2620f-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="2620f-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2620f-139">lastModifiedDateTime</span></span>|<span data-ttu-id="2620f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2620f-140">DateTimeOffset</span></span>|<span data-ttu-id="2620f-141">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2620f-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="2620f-142">version</span><span class="sxs-lookup"><span data-stu-id="2620f-142">version</span></span>|<span data-ttu-id="2620f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2620f-143">Int32</span></span>|<span data-ttu-id="2620f-144">Versão do CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="2620f-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="2620f-145">displayName</span><span class="sxs-lookup"><span data-stu-id="2620f-145">displayName</span></span>|<span data-ttu-id="2620f-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2620f-146">String</span></span>|<span data-ttu-id="2620f-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2620f-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="2620f-148">description</span><span class="sxs-lookup"><span data-stu-id="2620f-148">description</span></span>|<span data-ttu-id="2620f-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2620f-149">String</span></span>|<span data-ttu-id="2620f-150">Admin fornecido descrição do que o CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="2620f-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="2620f-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="2620f-151">deviceCartIds</span></span>|<span data-ttu-id="2620f-152">String collection</span><span class="sxs-lookup"><span data-stu-id="2620f-152">String collection</span></span>|<span data-ttu-id="2620f-153">Identificadores de carrinhos de dispositivo a ser associado a classes.</span><span class="sxs-lookup"><span data-stu-id="2620f-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="2620f-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="2620f-154">classroomIds</span></span>|<span data-ttu-id="2620f-155">String collection</span><span class="sxs-lookup"><span data-stu-id="2620f-155">String collection</span></span>|<span data-ttu-id="2620f-156">Identificadores de salas a ser associado ao dispositivo carrinhos de.</span><span class="sxs-lookup"><span data-stu-id="2620f-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="2620f-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="2620f-157">Response</span></span>
<span data-ttu-id="2620f-158">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2620f-158">If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2620f-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2620f-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="2620f-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2620f-160">Request</span></span>
<span data-ttu-id="2620f-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2620f-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
Content-type: application/json
Content-length: 335

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="2620f-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="2620f-162">Response</span></span>
<span data-ttu-id="2620f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2620f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "9bdc58dd-58dd-9bdc-dd58-dc9bdd58dc9b",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```





