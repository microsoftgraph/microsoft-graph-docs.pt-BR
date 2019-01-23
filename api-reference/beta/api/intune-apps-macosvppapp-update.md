---
title: Atualizar macOsVppApp
description: Atualize as propriedades de um objeto macOsVppApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b34a8e4ae3e179cfa8674abb08565b5fbe0c72a3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431277"
---
# <a name="update-macosvppapp"></a><span data-ttu-id="92e57-103">Atualizar macOsVppApp</span><span class="sxs-lookup"><span data-stu-id="92e57-103">Update macOsVppApp</span></span>

> <span data-ttu-id="92e57-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="92e57-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="92e57-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="92e57-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92e57-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="92e57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92e57-107">Atualize as propriedades de um objeto [macOsVppApp](../resources/intune-apps-macosvppapp.md) .</span><span class="sxs-lookup"><span data-stu-id="92e57-107">Update the properties of a [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92e57-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92e57-108">Prerequisites</span></span>
<span data-ttu-id="92e57-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="92e57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="92e57-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92e57-111">Permission type</span></span>|<span data-ttu-id="92e57-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92e57-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92e57-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92e57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92e57-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92e57-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="92e57-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92e57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92e57-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92e57-116">Not supported.</span></span>|
|<span data-ttu-id="92e57-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92e57-117">Application</span></span>|<span data-ttu-id="92e57-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92e57-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92e57-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92e57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="92e57-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92e57-120">Request headers</span></span>
|<span data-ttu-id="92e57-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92e57-121">Header</span></span>|<span data-ttu-id="92e57-122">Valor</span><span class="sxs-lookup"><span data-stu-id="92e57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92e57-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="92e57-123">Authorization</span></span>|<span data-ttu-id="92e57-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92e57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92e57-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92e57-125">Accept</span></span>|<span data-ttu-id="92e57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92e57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92e57-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92e57-127">Request body</span></span>
<span data-ttu-id="92e57-128">No corpo da solicitação, fornece uma representação JSON para o objeto [macOsVppApp](../resources/intune-apps-macosvppapp.md) .</span><span class="sxs-lookup"><span data-stu-id="92e57-128">In the request body, supply a JSON representation for the [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

<span data-ttu-id="92e57-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [macOsVppApp](../resources/intune-apps-macosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="92e57-129">The following table shows the properties that are required when you create the [macOsVppApp](../resources/intune-apps-macosvppapp.md).</span></span>

|<span data-ttu-id="92e57-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92e57-130">Property</span></span>|<span data-ttu-id="92e57-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="92e57-131">Type</span></span>|<span data-ttu-id="92e57-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="92e57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92e57-133">id</span><span class="sxs-lookup"><span data-stu-id="92e57-133">id</span></span>|<span data-ttu-id="92e57-134">String</span><span class="sxs-lookup"><span data-stu-id="92e57-134">String</span></span>|<span data-ttu-id="92e57-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="92e57-135">Key of the entity.</span></span> <span data-ttu-id="92e57-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92e57-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92e57-137">displayName</span><span class="sxs-lookup"><span data-stu-id="92e57-137">displayName</span></span>|<span data-ttu-id="92e57-138">String</span><span class="sxs-lookup"><span data-stu-id="92e57-138">String</span></span>|<span data-ttu-id="92e57-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="92e57-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="92e57-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92e57-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92e57-141">description</span><span class="sxs-lookup"><span data-stu-id="92e57-141">description</span></span>|<span data-ttu-id="92e57-142">String</span><span class="sxs-lookup"><span data-stu-id="92e57-142">String</span></span>|<span data-ttu-id="92e57-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92e57-143">The description of the app.</span></span> <span data-ttu-id="92e57-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92e57-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92e57-145">publisher</span><span class="sxs-lookup"><span data-stu-id="92e57-145">publisher</span></span>|<span data-ttu-id="92e57-146">String</span><span class="sxs-lookup"><span data-stu-id="92e57-146">String</span></span>|<span data-ttu-id="92e57-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92e57-147">The publisher of the app.</span></span> <span data-ttu-id="92e57-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92e57-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92e57-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="92e57-149">largeIcon</span></span>|[<span data-ttu-id="92e57-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="92e57-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="92e57-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="92e57-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="92e57-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92e57-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92e57-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92e57-153">createdDateTime</span></span>|<span data-ttu-id="92e57-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92e57-154">DateTimeOffset</span></span>|<span data-ttu-id="92e57-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92e57-155">The date and time the app was created.</span></span> <span data-ttu-id="92e57-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92e57-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92e57-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92e57-157">lastModifiedDateTime</span></span>|<span data-ttu-id="92e57-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92e57-158">DateTimeOffset</span></span>|<span data-ttu-id="92e57-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="92e57-159">The date and time the app was last modified.</span></span> <span data-ttu-id="92e57-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92e57-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92e57-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="92e57-161">isFeatured</span></span>|<span data-ttu-id="92e57-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="92e57-162">Boolean</span></span>|<span data-ttu-id="92e57-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92e57-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92e57-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="92e57-164">privacyInformationUrl</span></span>|<span data-ttu-id="92e57-165">String</span><span class="sxs-lookup"><span data-stu-id="92e57-165">String</span></span>|<span data-ttu-id="92e57-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="92e57-166">The privacy statement Url.</span></span> <span data-ttu-id="92e57-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92e57-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92e57-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="92e57-168">informationUrl</span></span>|<span data-ttu-id="92e57-169">String</span><span class="sxs-lookup"><span data-stu-id="92e57-169">String</span></span>|<span data-ttu-id="92e57-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="92e57-170">The more information Url.</span></span> <span data-ttu-id="92e57-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92e57-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92e57-172">owner</span><span class="sxs-lookup"><span data-stu-id="92e57-172">owner</span></span>|<span data-ttu-id="92e57-173">String</span><span class="sxs-lookup"><span data-stu-id="92e57-173">String</span></span>|<span data-ttu-id="92e57-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="92e57-174">The owner of the app.</span></span> <span data-ttu-id="92e57-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92e57-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92e57-176">developer</span><span class="sxs-lookup"><span data-stu-id="92e57-176">developer</span></span>|<span data-ttu-id="92e57-177">String</span><span class="sxs-lookup"><span data-stu-id="92e57-177">String</span></span>|<span data-ttu-id="92e57-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92e57-178">The developer of the app.</span></span> <span data-ttu-id="92e57-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92e57-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92e57-180">Observações</span><span class="sxs-lookup"><span data-stu-id="92e57-180">notes</span></span>|<span data-ttu-id="92e57-181">String</span><span class="sxs-lookup"><span data-stu-id="92e57-181">String</span></span>|<span data-ttu-id="92e57-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92e57-182">Notes for the app.</span></span> <span data-ttu-id="92e57-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92e57-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92e57-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="92e57-184">uploadState</span></span>|<span data-ttu-id="92e57-185">Int32</span><span class="sxs-lookup"><span data-stu-id="92e57-185">Int32</span></span>|<span data-ttu-id="92e57-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="92e57-186">The upload state.</span></span> <span data-ttu-id="92e57-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92e57-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92e57-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="92e57-188">publishingState</span></span>|[<span data-ttu-id="92e57-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="92e57-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="92e57-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92e57-190">The publishing state for the app.</span></span> <span data-ttu-id="92e57-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="92e57-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="92e57-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92e57-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="92e57-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="92e57-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="92e57-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="92e57-194">isAssigned</span></span>|<span data-ttu-id="92e57-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="92e57-195">Boolean</span></span>|<span data-ttu-id="92e57-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="92e57-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="92e57-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92e57-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92e57-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="92e57-198">roleScopeTagIds</span></span>|<span data-ttu-id="92e57-199">String collection</span><span class="sxs-lookup"><span data-stu-id="92e57-199">String collection</span></span>|<span data-ttu-id="92e57-200">Lista de ids de marca de escopo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="92e57-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="92e57-201">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92e57-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92e57-202">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="92e57-202">usedLicenseCount</span></span>|<span data-ttu-id="92e57-203">Int32</span><span class="sxs-lookup"><span data-stu-id="92e57-203">Int32</span></span>|<span data-ttu-id="92e57-204">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="92e57-204">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="92e57-205">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="92e57-205">totalLicenseCount</span></span>|<span data-ttu-id="92e57-206">Int32</span><span class="sxs-lookup"><span data-stu-id="92e57-206">Int32</span></span>|<span data-ttu-id="92e57-207">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="92e57-207">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="92e57-208">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="92e57-208">releaseDateTime</span></span>|<span data-ttu-id="92e57-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92e57-209">DateTimeOffset</span></span>|<span data-ttu-id="92e57-210">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="92e57-210">The VPP application release date and time.</span></span>|
|<span data-ttu-id="92e57-211">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="92e57-211">appStoreUrl</span></span>|<span data-ttu-id="92e57-212">String</span><span class="sxs-lookup"><span data-stu-id="92e57-212">String</span></span>|<span data-ttu-id="92e57-213">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="92e57-213">The store URL.</span></span>|
|<span data-ttu-id="92e57-214">licensingType</span><span class="sxs-lookup"><span data-stu-id="92e57-214">licensingType</span></span>|[<span data-ttu-id="92e57-215">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="92e57-215">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="92e57-216">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="92e57-216">The supported License Type.</span></span>|
|<span data-ttu-id="92e57-217">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="92e57-217">vppTokenOrganizationName</span></span>|<span data-ttu-id="92e57-218">String</span><span class="sxs-lookup"><span data-stu-id="92e57-218">String</span></span>|<span data-ttu-id="92e57-219">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="92e57-219">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="92e57-220">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="92e57-220">vppTokenAccountType</span></span>|[<span data-ttu-id="92e57-221">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="92e57-221">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="92e57-222">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="92e57-222">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="92e57-223">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="92e57-223">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="92e57-224">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="92e57-224">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="92e57-225">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="92e57-225">vppTokenAppleId</span></span>|<span data-ttu-id="92e57-226">String</span><span class="sxs-lookup"><span data-stu-id="92e57-226">String</span></span>|<span data-ttu-id="92e57-227">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="92e57-227">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="92e57-228">bundleId</span><span class="sxs-lookup"><span data-stu-id="92e57-228">bundleId</span></span>|<span data-ttu-id="92e57-229">String</span><span class="sxs-lookup"><span data-stu-id="92e57-229">String</span></span>|<span data-ttu-id="92e57-230">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="92e57-230">The Identity Name.</span></span>|
|<span data-ttu-id="92e57-231">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="92e57-231">vppTokenId</span></span>|<span data-ttu-id="92e57-232">String</span><span class="sxs-lookup"><span data-stu-id="92e57-232">String</span></span>|<span data-ttu-id="92e57-233">Identificador do token VPP associado a esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92e57-233">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="92e57-234">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="92e57-234">revokeLicenseActionResults</span></span>|<span data-ttu-id="92e57-235">coleção [macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="92e57-235">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="92e57-236">Resultados de revogar ações de licença em deste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92e57-236">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="92e57-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="92e57-237">Response</span></span>
<span data-ttu-id="92e57-238">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [macOsVppApp](../resources/intune-apps-macosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92e57-238">If successful, this method returns a `200 OK` response code and an updated [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92e57-239">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92e57-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="92e57-240">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92e57-240">Request</span></span>
<span data-ttu-id="92e57-241">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92e57-241">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1842

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
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
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
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

### <a name="response"></a><span data-ttu-id="92e57-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="92e57-242">Response</span></span>
<span data-ttu-id="92e57-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92e57-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2014

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
  "id": "10b95265-5265-10b9-6552-b9106552b910",
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
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
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




