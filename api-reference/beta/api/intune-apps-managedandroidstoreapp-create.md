---
title: Criar managedAndroidStoreApp
description: Cria um novo objeto managedAndroidStoreApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a7bd4cf3b84140c61cdd84b024c6574271440620
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405202"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="c1ac3-103">Criar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="c1ac3-103">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="c1ac3-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c1ac3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1ac3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1ac3-107">Cria um novo objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ac3-107">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1ac3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c1ac3-108">Prerequisites</span></span>
<span data-ttu-id="c1ac3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c1ac3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c1ac3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1ac3-111">Permission type</span></span>|<span data-ttu-id="c1ac3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1ac3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1ac3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1ac3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c1ac3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1ac3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-116">Not supported.</span></span>|
|<span data-ttu-id="c1ac3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1ac3-117">Application</span></span>|<span data-ttu-id="c1ac3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1ac3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1ac3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c1ac3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1ac3-120">Request headers</span></span>
|<span data-ttu-id="c1ac3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c1ac3-121">Header</span></span>|<span data-ttu-id="c1ac3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c1ac3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1ac3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1ac3-123">Authorization</span></span>|<span data-ttu-id="c1ac3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1ac3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c1ac3-125">Accept</span></span>|<span data-ttu-id="c1ac3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1ac3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1ac3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1ac3-127">Request body</span></span>
<span data-ttu-id="c1ac3-128">No corpo da solicitação, forneça uma representação JSON do objeto managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-128">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="c1ac3-129">A tabela a seguir mostra as propriedades obrigatórias ao criar managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-129">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="c1ac3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1ac3-130">Property</span></span>|<span data-ttu-id="c1ac3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1ac3-131">Type</span></span>|<span data-ttu-id="c1ac3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1ac3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1ac3-133">id</span><span class="sxs-lookup"><span data-stu-id="c1ac3-133">id</span></span>|<span data-ttu-id="c1ac3-134">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-134">String</span></span>|<span data-ttu-id="c1ac3-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-135">Key of the entity.</span></span> <span data-ttu-id="c1ac3-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ac3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c1ac3-137">displayName</span></span>|<span data-ttu-id="c1ac3-138">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-138">String</span></span>|<span data-ttu-id="c1ac3-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c1ac3-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ac3-141">description</span><span class="sxs-lookup"><span data-stu-id="c1ac3-141">description</span></span>|<span data-ttu-id="c1ac3-142">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-142">String</span></span>|<span data-ttu-id="c1ac3-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-143">The description of the app.</span></span> <span data-ttu-id="c1ac3-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ac3-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c1ac3-145">publisher</span></span>|<span data-ttu-id="c1ac3-146">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-146">String</span></span>|<span data-ttu-id="c1ac3-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-147">The publisher of the app.</span></span> <span data-ttu-id="c1ac3-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ac3-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c1ac3-149">largeIcon</span></span>|[<span data-ttu-id="c1ac3-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c1ac3-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c1ac3-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c1ac3-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ac3-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1ac3-153">createdDateTime</span></span>|<span data-ttu-id="c1ac3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1ac3-154">DateTimeOffset</span></span>|<span data-ttu-id="c1ac3-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-155">The date and time the app was created.</span></span> <span data-ttu-id="c1ac3-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ac3-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1ac3-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c1ac3-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1ac3-158">DateTimeOffset</span></span>|<span data-ttu-id="c1ac3-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c1ac3-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ac3-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c1ac3-161">isFeatured</span></span>|<span data-ttu-id="c1ac3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1ac3-162">Boolean</span></span>|<span data-ttu-id="c1ac3-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ac3-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c1ac3-164">privacyInformationUrl</span></span>|<span data-ttu-id="c1ac3-165">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-165">String</span></span>|<span data-ttu-id="c1ac3-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-166">The privacy statement Url.</span></span> <span data-ttu-id="c1ac3-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ac3-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c1ac3-168">informationUrl</span></span>|<span data-ttu-id="c1ac3-169">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-169">String</span></span>|<span data-ttu-id="c1ac3-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-170">The more information Url.</span></span> <span data-ttu-id="c1ac3-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ac3-172">owner</span><span class="sxs-lookup"><span data-stu-id="c1ac3-172">owner</span></span>|<span data-ttu-id="c1ac3-173">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-173">String</span></span>|<span data-ttu-id="c1ac3-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-174">The owner of the app.</span></span> <span data-ttu-id="c1ac3-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ac3-176">developer</span><span class="sxs-lookup"><span data-stu-id="c1ac3-176">developer</span></span>|<span data-ttu-id="c1ac3-177">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-177">String</span></span>|<span data-ttu-id="c1ac3-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-178">The developer of the app.</span></span> <span data-ttu-id="c1ac3-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ac3-180">Observações</span><span class="sxs-lookup"><span data-stu-id="c1ac3-180">notes</span></span>|<span data-ttu-id="c1ac3-181">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-181">String</span></span>|<span data-ttu-id="c1ac3-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-182">Notes for the app.</span></span> <span data-ttu-id="c1ac3-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ac3-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c1ac3-184">uploadState</span></span>|<span data-ttu-id="c1ac3-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c1ac3-185">Int32</span></span>|<span data-ttu-id="c1ac3-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-186">The upload state.</span></span> <span data-ttu-id="c1ac3-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ac3-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="c1ac3-188">publishingState</span></span>|[<span data-ttu-id="c1ac3-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c1ac3-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c1ac3-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-190">The publishing state for the app.</span></span> <span data-ttu-id="c1ac3-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c1ac3-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ac3-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c1ac3-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c1ac3-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c1ac3-194">isAssigned</span></span>|<span data-ttu-id="c1ac3-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1ac3-195">Boolean</span></span>|<span data-ttu-id="c1ac3-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c1ac3-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ac3-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c1ac3-198">roleScopeTagIds</span></span>|<span data-ttu-id="c1ac3-199">String collection</span><span class="sxs-lookup"><span data-stu-id="c1ac3-199">String collection</span></span>|<span data-ttu-id="c1ac3-200">Lista de ids de marca de escopo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c1ac3-201">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ac3-202">appAvailability</span><span class="sxs-lookup"><span data-stu-id="c1ac3-202">appAvailability</span></span>|[<span data-ttu-id="c1ac3-203">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="c1ac3-203">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="c1ac3-204">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-204">The Application's availability.</span></span> <span data-ttu-id="c1ac3-205">Herdada do [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ac3-205">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="c1ac3-206">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-206">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="c1ac3-207">version</span><span class="sxs-lookup"><span data-stu-id="c1ac3-207">version</span></span>|<span data-ttu-id="c1ac3-208">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-208">String</span></span>|<span data-ttu-id="c1ac3-209">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-209">The Application's version.</span></span> <span data-ttu-id="c1ac3-210">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="c1ac3-211">packageId</span><span class="sxs-lookup"><span data-stu-id="c1ac3-211">packageId</span></span>|<span data-ttu-id="c1ac3-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1ac3-212">String</span></span>|<span data-ttu-id="c1ac3-213">A ID de pacote do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-213">The app's package ID.</span></span>|
|<span data-ttu-id="c1ac3-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c1ac3-214">appStoreUrl</span></span>|<span data-ttu-id="c1ac3-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1ac3-215">String</span></span>|<span data-ttu-id="c1ac3-216">A AppStoreUrl do Android.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-216">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="c1ac3-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c1ac3-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c1ac3-218">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c1ac3-218">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="c1ac3-219">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-219">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="c1ac3-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1ac3-220">Response</span></span>
<span data-ttu-id="c1ac3-221">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-221">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1ac3-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1ac3-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1ac3-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1ac3-223">Request</span></span>
<span data-ttu-id="c1ac3-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1237

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="c1ac3-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1ac3-225">Response</span></span>
<span data-ttu-id="c1ac3-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1409

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```




