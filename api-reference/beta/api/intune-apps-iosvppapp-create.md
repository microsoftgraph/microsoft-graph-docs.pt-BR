---
title: Criar iosVppApp
description: Cria um novo objeto iosVppApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8e9ad9c99835a138dc5de52c1008b1e2ba24607f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424536"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="00bd4-103">Criar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="00bd4-103">Create iosVppApp</span></span>

> <span data-ttu-id="00bd4-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="00bd4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="00bd4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="00bd4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00bd4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="00bd4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00bd4-107">Cria um novo objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="00bd4-107">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00bd4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="00bd4-108">Prerequisites</span></span>
<span data-ttu-id="00bd4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="00bd4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="00bd4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00bd4-111">Permission type</span></span>|<span data-ttu-id="00bd4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="00bd4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00bd4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00bd4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00bd4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00bd4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="00bd4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00bd4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00bd4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00bd4-116">Not supported.</span></span>|
|<span data-ttu-id="00bd4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00bd4-117">Application</span></span>|<span data-ttu-id="00bd4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00bd4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00bd4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00bd4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="00bd4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00bd4-120">Request headers</span></span>
|<span data-ttu-id="00bd4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="00bd4-121">Header</span></span>|<span data-ttu-id="00bd4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="00bd4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00bd4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="00bd4-123">Authorization</span></span>|<span data-ttu-id="00bd4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00bd4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00bd4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="00bd4-125">Accept</span></span>|<span data-ttu-id="00bd4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00bd4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00bd4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00bd4-127">Request body</span></span>
<span data-ttu-id="00bd4-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="00bd4-128">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="00bd4-129">A tabela a seguir mostra as propriedades obrigatórias ao criar iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="00bd4-129">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="00bd4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00bd4-130">Property</span></span>|<span data-ttu-id="00bd4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="00bd4-131">Type</span></span>|<span data-ttu-id="00bd4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="00bd4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00bd4-133">id</span><span class="sxs-lookup"><span data-stu-id="00bd4-133">id</span></span>|<span data-ttu-id="00bd4-134">String</span><span class="sxs-lookup"><span data-stu-id="00bd4-134">String</span></span>|<span data-ttu-id="00bd4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="00bd4-135">Key of the entity.</span></span> <span data-ttu-id="00bd4-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00bd4-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00bd4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="00bd4-137">displayName</span></span>|<span data-ttu-id="00bd4-138">String</span><span class="sxs-lookup"><span data-stu-id="00bd4-138">String</span></span>|<span data-ttu-id="00bd4-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="00bd4-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="00bd4-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00bd4-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00bd4-141">description</span><span class="sxs-lookup"><span data-stu-id="00bd4-141">description</span></span>|<span data-ttu-id="00bd4-142">String</span><span class="sxs-lookup"><span data-stu-id="00bd4-142">String</span></span>|<span data-ttu-id="00bd4-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00bd4-143">The description of the app.</span></span> <span data-ttu-id="00bd4-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00bd4-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00bd4-145">publisher</span><span class="sxs-lookup"><span data-stu-id="00bd4-145">publisher</span></span>|<span data-ttu-id="00bd4-146">String</span><span class="sxs-lookup"><span data-stu-id="00bd4-146">String</span></span>|<span data-ttu-id="00bd4-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00bd4-147">The publisher of the app.</span></span> <span data-ttu-id="00bd4-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00bd4-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00bd4-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="00bd4-149">largeIcon</span></span>|[<span data-ttu-id="00bd4-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="00bd4-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="00bd4-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="00bd4-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="00bd4-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00bd4-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00bd4-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00bd4-153">createdDateTime</span></span>|<span data-ttu-id="00bd4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00bd4-154">DateTimeOffset</span></span>|<span data-ttu-id="00bd4-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00bd4-155">The date and time the app was created.</span></span> <span data-ttu-id="00bd4-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00bd4-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00bd4-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00bd4-157">lastModifiedDateTime</span></span>|<span data-ttu-id="00bd4-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00bd4-158">DateTimeOffset</span></span>|<span data-ttu-id="00bd4-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="00bd4-159">The date and time the app was last modified.</span></span> <span data-ttu-id="00bd4-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00bd4-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00bd4-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="00bd4-161">isFeatured</span></span>|<span data-ttu-id="00bd4-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="00bd4-162">Boolean</span></span>|<span data-ttu-id="00bd4-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00bd4-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00bd4-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="00bd4-164">privacyInformationUrl</span></span>|<span data-ttu-id="00bd4-165">String</span><span class="sxs-lookup"><span data-stu-id="00bd4-165">String</span></span>|<span data-ttu-id="00bd4-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="00bd4-166">The privacy statement Url.</span></span> <span data-ttu-id="00bd4-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00bd4-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00bd4-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="00bd4-168">informationUrl</span></span>|<span data-ttu-id="00bd4-169">String</span><span class="sxs-lookup"><span data-stu-id="00bd4-169">String</span></span>|<span data-ttu-id="00bd4-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="00bd4-170">The more information Url.</span></span> <span data-ttu-id="00bd4-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00bd4-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00bd4-172">owner</span><span class="sxs-lookup"><span data-stu-id="00bd4-172">owner</span></span>|<span data-ttu-id="00bd4-173">String</span><span class="sxs-lookup"><span data-stu-id="00bd4-173">String</span></span>|<span data-ttu-id="00bd4-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="00bd4-174">The owner of the app.</span></span> <span data-ttu-id="00bd4-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00bd4-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00bd4-176">developer</span><span class="sxs-lookup"><span data-stu-id="00bd4-176">developer</span></span>|<span data-ttu-id="00bd4-177">String</span><span class="sxs-lookup"><span data-stu-id="00bd4-177">String</span></span>|<span data-ttu-id="00bd4-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00bd4-178">The developer of the app.</span></span> <span data-ttu-id="00bd4-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00bd4-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00bd4-180">Observações</span><span class="sxs-lookup"><span data-stu-id="00bd4-180">notes</span></span>|<span data-ttu-id="00bd4-181">String</span><span class="sxs-lookup"><span data-stu-id="00bd4-181">String</span></span>|<span data-ttu-id="00bd4-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00bd4-182">Notes for the app.</span></span> <span data-ttu-id="00bd4-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00bd4-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00bd4-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="00bd4-184">uploadState</span></span>|<span data-ttu-id="00bd4-185">Int32</span><span class="sxs-lookup"><span data-stu-id="00bd4-185">Int32</span></span>|<span data-ttu-id="00bd4-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="00bd4-186">The upload state.</span></span> <span data-ttu-id="00bd4-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00bd4-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00bd4-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="00bd4-188">publishingState</span></span>|[<span data-ttu-id="00bd4-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="00bd4-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="00bd4-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00bd4-190">The publishing state for the app.</span></span> <span data-ttu-id="00bd4-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="00bd4-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="00bd4-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00bd4-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="00bd4-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="00bd4-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="00bd4-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="00bd4-194">isAssigned</span></span>|<span data-ttu-id="00bd4-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="00bd4-195">Boolean</span></span>|<span data-ttu-id="00bd4-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="00bd4-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="00bd4-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00bd4-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00bd4-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="00bd4-198">roleScopeTagIds</span></span>|<span data-ttu-id="00bd4-199">String collection</span><span class="sxs-lookup"><span data-stu-id="00bd4-199">String collection</span></span>|<span data-ttu-id="00bd4-200">Lista de ids de marca de escopo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="00bd4-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="00bd4-201">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00bd4-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00bd4-202">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="00bd4-202">usedLicenseCount</span></span>|<span data-ttu-id="00bd4-203">Int32</span><span class="sxs-lookup"><span data-stu-id="00bd4-203">Int32</span></span>|<span data-ttu-id="00bd4-204">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="00bd4-204">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="00bd4-205">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="00bd4-205">totalLicenseCount</span></span>|<span data-ttu-id="00bd4-206">Int32</span><span class="sxs-lookup"><span data-stu-id="00bd4-206">Int32</span></span>|<span data-ttu-id="00bd4-207">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="00bd4-207">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="00bd4-208">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="00bd4-208">releaseDateTime</span></span>|<span data-ttu-id="00bd4-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00bd4-209">DateTimeOffset</span></span>|<span data-ttu-id="00bd4-210">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="00bd4-210">The VPP application release date and time.</span></span>|
|<span data-ttu-id="00bd4-211">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="00bd4-211">appStoreUrl</span></span>|<span data-ttu-id="00bd4-212">String</span><span class="sxs-lookup"><span data-stu-id="00bd4-212">String</span></span>|<span data-ttu-id="00bd4-213">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="00bd4-213">The store URL.</span></span>|
|<span data-ttu-id="00bd4-214">licensingType</span><span class="sxs-lookup"><span data-stu-id="00bd4-214">licensingType</span></span>|[<span data-ttu-id="00bd4-215">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="00bd4-215">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="00bd4-216">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="00bd4-216">The supported License Type.</span></span>|
|<span data-ttu-id="00bd4-217">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="00bd4-217">applicableDeviceType</span></span>|[<span data-ttu-id="00bd4-218">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="00bd4-218">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="00bd4-219">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="00bd4-219">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="00bd4-220">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="00bd4-220">vppTokenOrganizationName</span></span>|<span data-ttu-id="00bd4-221">String</span><span class="sxs-lookup"><span data-stu-id="00bd4-221">String</span></span>|<span data-ttu-id="00bd4-222">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="00bd4-222">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="00bd4-223">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="00bd4-223">vppTokenAccountType</span></span>|[<span data-ttu-id="00bd4-224">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="00bd4-224">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="00bd4-225">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="00bd4-225">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="00bd4-226">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="00bd4-226">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="00bd4-227">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="00bd4-227">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="00bd4-228">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="00bd4-228">vppTokenAppleId</span></span>|<span data-ttu-id="00bd4-229">String</span><span class="sxs-lookup"><span data-stu-id="00bd4-229">String</span></span>|<span data-ttu-id="00bd4-230">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="00bd4-230">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="00bd4-231">bundleId</span><span class="sxs-lookup"><span data-stu-id="00bd4-231">bundleId</span></span>|<span data-ttu-id="00bd4-232">String</span><span class="sxs-lookup"><span data-stu-id="00bd4-232">String</span></span>|<span data-ttu-id="00bd4-233">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="00bd4-233">The Identity Name.</span></span>|
|<span data-ttu-id="00bd4-234">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="00bd4-234">vppTokenId</span></span>|<span data-ttu-id="00bd4-235">String</span><span class="sxs-lookup"><span data-stu-id="00bd4-235">String</span></span>|<span data-ttu-id="00bd4-236">Identificador do token VPP associado a esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00bd4-236">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="00bd4-237">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="00bd4-237">revokeLicenseActionResults</span></span>|<span data-ttu-id="00bd4-238">coleção [iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="00bd4-238">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="00bd4-239">Resultados de revogar ações de licença em deste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00bd4-239">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="00bd4-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="00bd4-240">Response</span></span>
<span data-ttu-id="00bd4-241">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00bd4-241">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00bd4-242">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00bd4-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="00bd4-243">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00bd4-243">Request</span></span>
<span data-ttu-id="00bd4-244">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00bd4-244">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1972

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="00bd4-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="00bd4-245">Response</span></span>
<span data-ttu-id="00bd4-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00bd4-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2144

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```




