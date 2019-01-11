---
title: Controle de acesso baseado em função no Microsoft Intune
description: 'O controle de acesso baseado em função do Intune determina quem pode executar ações em objetos do Intune e fazer alterações para aplicativos gerenciados, usuários e dispositivos.   '
localization_priority: Normal
ms.openlocfilehash: 7772ad42d96f6c8907f813e8e62cfb4429fe2cc2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804883"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="bbd4c-103">Controle de acesso baseado em função no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bbd4c-103">Role-based access control in Microsoft Intune</span></span>

> <span data-ttu-id="bbd4c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bbd4c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbd4c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bbd4c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bbd4c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bbd4c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="bbd4c-107">O controle de acesso baseado em função do Intune determina quem pode executar ações em objetos do Intune e fazer alterações para aplicativos gerenciados, usuários e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="bbd4c-107">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="bbd4c-108">Os seguintes recursos do Graph estão disponíveis para gerenciar o controle de acesso baseado em função no Intune:</span><span class="sxs-lookup"><span data-stu-id="bbd4c-108">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="bbd4c-109">Gerenciamento de dispositivo e app atribuídas identificações de função</span><span class="sxs-lookup"><span data-stu-id="bbd4c-109">Device and app management assigned role ids</span></span>](intune-rbac-deviceandappmanagementassignedroleids.md)
- [<span data-ttu-id="bbd4c-110">Atribuição de função de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="bbd4c-110">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="bbd4c-111">Definição de função de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="bbd4c-111">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="bbd4c-112">Ação de recurso</span><span class="sxs-lookup"><span data-stu-id="bbd4c-112">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="bbd4c-113">Operação de recurso</span><span class="sxs-lookup"><span data-stu-id="bbd4c-113">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="bbd4c-114">Atribuição de função</span><span class="sxs-lookup"><span data-stu-id="bbd4c-114">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="bbd4c-115">Tipo de escopo de atribuição de função</span><span class="sxs-lookup"><span data-stu-id="bbd4c-115">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="bbd4c-116">Definição de função</span><span class="sxs-lookup"><span data-stu-id="bbd4c-116">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="bbd4c-117">Permissão de função</span><span class="sxs-lookup"><span data-stu-id="bbd4c-117">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="bbd4c-118">Marca de escopo de função</span><span class="sxs-lookup"><span data-stu-id="bbd4c-118">Role scope tag</span></span>](intune-rbac-rolescopetag.md)
