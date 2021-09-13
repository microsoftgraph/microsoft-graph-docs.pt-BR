---
title: Gerenciamento de despesas de telecomunicações em Microsoft Intune - API Graph Microsoft
description: Lista a API Graph microsoft para pontos de extremidade do Intune (REST) relacionadas ao gerenciamento de despesas de telecomunicações para uma organização de locatários.
ms.localizationpriority: medium
author: dougeby
ms.prod: intune
ms.openlocfilehash: e5ba17fb120ea4599dd31ffaab58ff12397b450f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039018"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a>Gerenciamento de despesas com telecomunicações no Microsoft Intune

Namespace: microsoft.graph

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

É possível limitar o uso e o roaming de dados em dispositivos de propriedade corporativa ao usar o serviço de gerenciamento de despesas com telecomunicações Saaswedo, que é integrado ao Intune. O serviço permite configurar e impor limites de uso e enviar aos usuários um alerta quando eles excederem um limite configurado. Também é possível configurar o serviço para realizar outras ações, como a desabilitação do roaming, quando os usuários excederem o limite. Relatórios com informações sobre o uso e o monitoramento dos dados estão disponíveis no console do Saaswedo. Antes de usar o serviço de gerenciamento de despesas com telecomunicações Saaswedo com o Intune, é preciso definir as configurações em um console do Saaswedo e no Intune. A conexão deve ser ativada para o serviço Saaswedo e para o Intune. Se a conexão do lado do Saaswedo estiver habilitada, mas a do lado do Intune não estiver, o Intune receberá a comunicação, mas ela será ignorada.

Os seguintes recursos do Graph estão disponíveis para gerenciar despesas com telecomunicações no Intune:

- [Parceiro de gerenciamento de despesas com telecomunicações](intune-tem-telecomexpensemanagementpartner.md)
